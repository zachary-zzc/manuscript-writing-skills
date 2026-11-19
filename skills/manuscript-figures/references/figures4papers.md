# Python manuscript figures with figures4papers

Use this reference when creating or revising static manuscript plots in Python/Matplotlib. Read [figures.md](figures.md) for the scientific and visual requirements. Keep the task's confirmed Easy, Normal or Expert mode; this helper adds no intake or approval checkpoints. Keep an existing R or vector workflow when it fits the requested output. Interactive Crux bundles remain with the Crux workflow.

This is a local adaptation of Chen Liu's [figures4papers scientific-figure-making skill](https://github.com/ChenLiu-1996/figures4papers/blob/main/scientific-figure-making/SKILL.md), reviewed on 28 October 2026 from `main`. The links follow upstream `main`; they are not a pinned release or automatic update. The source uses [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/); see its [license and warranty disclaimer](https://github.com/ChenLiu-1996/figures4papers/blob/main/LICENSE). Retain attribution, license links and modification notices when sharing adapted material. Commercial reuse of upstream licensed material requires separate permission. This adaptation makes the house style optional and adds manuscript-specific evidence and axis safeguards; it does not change the license of unrelated workflow material.

## Choose a pattern from the scientific comparison

| Plot | Implementation decision |
|---|---|
| Grouped bars or ablations | Align every series to one explicit category order. Compute offsets from the number of series; keep labels, colours and annotations attached to the correct series. Use edges or hatching when fills alone are ambiguous in print. |
| Trends | Use actual x coordinates and an explicit ordering. Distinguish series with both colour and line/marker encodings when useful. A shared legend can occupy a spare grid cell. |
| Heatmaps | Validate matrix dimensions against row/column labels. Label the colourbar with the quantity and units. Share limits across comparable panels; use a meaningful centre for signed quantities and distinguish missing cells from zero. |
| Scatter | Validate paired coordinates and preserve the observation unit. Use transparency or selective rasterization for density while retaining readable labels and vector axes. |
| Radar/polar | Use only when the comparison benefits from it. State normalization, direction of improvement and axis order; do not connect unrelated metric scales without an explicit transformation. |

The upstream [pattern guide](https://github.com/ChenLiu-1996/figures4papers/blob/main/scientific-figure-making/references/common-patterns.md) supplies layout and print-encoding ideas. Apply these qualifications:

- Bars encode magnitude by length: normally retain zero and include negative values and intervals. For close differences, prefer a dot/interval plot or a clearly disclosed inset or axis break over silently truncating bars. Line and scatter limits may follow the relevant range when they preserve the comparison and all relevant evidence.
- An uncertainty band needs actual bounds or a justified calculation from replicates, with the statistic and sampling unit recorded. A helper's `show_shadow` option is not evidence of uncertainty. Do not manufacture bands, significance marks or replicates.
- Hide category ticks only when each mark remains unambiguously identifiable. Collect and deduplicate legend entries across all panels; the first panel may not contain every series.
- Tutorial arrays and random matrices are demonstration data. They are not study results or measured correlations. Keep any synthetic layout preview explicitly labelled and separate from the submission figure.

## Implement reproducibly in the manuscript project

The upstream [API reference](https://github.com/ChenLiu-1996/figures4papers/blob/main/scientific-figure-making/references/api.md) describes helpers to implement. It does not supply an importable shared plotting package. Use existing project helpers or implement only the needed functions; do not install a presumed `figures4papers` Python package or call undefined tutorial functions.

Useful separations are a project style configuration, plot functions receiving an `Axes`, and one export function. The upstream names `apply_publication_style`, `make_grouped_bar`, `make_trend`, `make_heatmap` and `finalize_figure` are optional conventions. If following them, verify their actual return values: the documented grouped-bar helper returns only the last bar container, so it is insufficient for annotating every series without adaptation.

Keep source-data loading, analysis transformations and rendering separable. Check array shapes, label counts, missing-value handling and series order before plotting. Preserve source values and record any filtering, aggregation or normalization in the reproducible script. Use NumPy and Matplotlib where sufficient; inspect an example's imports before adding any other dependency.

For unattended execution, select a non-interactive backend before importing `pyplot`. Resolve input and output locations explicitly, use stable output names, and retain the runnable script with the manuscript. Reuse the project's environment and record the dependencies needed to reproduce the figure.

## Fit the manuscript's visual profile

Use the accepted manuscript profile and verified venue specifications for physical dimensions, typography, line weights and output settings. The [upstream design guide](https://github.com/ChenLiu-1996/figures4papers/blob/main/scientific-figure-making/references/design-theory.md) offers style examples, not universal journal requirements. Its large canvases, font sizes, Helvetica preference and palette must not override that profile.

Maintain a stable mapping from scientific categories to colours across figures. Do not automatically colour a proposed method blue, comparators red or improvements green when the manuscript already assigns different meanings. Check contrast and redundant encodings at final size. Reserve a legend area when needed rather than covering data; do not enlarge the canvas indefinitely to fit labels.

Apply style through a scoped configuration such as `matplotlib.rc_context` when several figure styles share a process. Use installed font fallbacks and verify glyphs. Enable external TeX only when required and available; ordinary mathematical labels do not by themselves require it.

## Export and inspect

Produce the requested submission format and an inspectable preview; PDF plus PNG is a useful starting pair when formats are unspecified. SVG can preserve editable text with `svg.fonttype = 'none'`, but font portability still needs checking. Set raster resolution for the final physical size; DPI does not improve vector paths or recover missing image detail.

Have the export helper create the output directory, save each requested format and return the actual paths. Verify layout after legends, annotations and colourbars are present. Tight bounding-box cropping can change physical dimensions, so inspect the saved dimensions and the manuscript insertion. Run the script and inspect its actual exports before reporting success; use the four-layer checks in [audit.md](../../manuscript-audit/references/audit.md).

For a worked starting point, load the upstream [tutorials](https://github.com/ChenLiu-1996/figures4papers/blob/main/scientific-figure-making/references/tutorials.md) only for the relevant chart. The [demo index](https://github.com/ChenLiu-1996/figures4papers/blob/main/scientific-figure-making/references/demos.md) points to comparison bars, trends, heatmaps and radar scripts. Inspect only a matching example, record its commit when copying material, preserve its license notice, and replace its project paths and demonstration data with the manuscript's actual inputs. This local reference is sufficient for routine plotting without fetching those examples.
