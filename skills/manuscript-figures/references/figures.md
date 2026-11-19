# Scientific figure generation

Use for new scientific figures, substantive redesigns and figure-set planning. Apply the confirmed interaction mode to storyboard, prototype and draft reviews; these design steps do not add approval prompts to Easy. Preserve protected artwork and original evaluated outputs. Audit generated work with [audit.md](../../manuscript-audit/references/audit.md).

Before selecting a chart form for a new or redesigned main figure, read [visual-form-selection.md](visual-form-selection.md). The selection record is part of the panel plan.

## Purpose and data

1. **Define the question.** Give each panel a specific scientific question, supported finding and role in the accepted storyline. Connect it to the main result and adjacent panels. Resolve an unclear purpose before drawing; a capability description or activity count cannot substitute for the scientific outcome.

2. **Inspect the data before choosing an encoding.** Establish observational unit, variable types, available rows, repeated measurements, hierarchy, relationships, sample size, missingness and comparison. Bind the panel to its actual source, population and transformation. Do not choose a compelling visual first and invent the required distribution afterward.

3. **Preserve meaningful biological structure.** Show pathways, modules, trees, networks, genome organisation or host relationships when these carry the evidence. Counts alone may erase that structure. Add relationship diagrams only when the relationships are supported and help communicate the finding. For biological or computational schematics, apply the [component and edge checks](figure-verification.md#schematic-components-and-edges).

4. **Interpret complexity as information.** Richer visualizations should expose relationships, distributions, multivariate patterns or biological interpretation. Extra decoration, marks and nodes alone add little. Choose sophistication for the question and audience; neither maximal density nor minimalism is the objective.

5. **Assign distinct evidentiary roles.** A composite can connect context, primary evidence, comparison, qualification and implication. Remove redundant or trivial panels while preserving important null findings. Reuse an encoding when it aids comparison; converting every bar into the same lollipop chart provides cosmetic variety only.

6. **Match form to quantity and scale.** Use direct labels for manageable sets, aligned points or facets for comparisons, and appropriate distribution summaries for shape, tails or thresholds. Larger sets may need justified aggregation or binning. Record those transformations. No universal mark count determines whether a panel is meaningful.

7. **Show findings rather than task activity.** Biological figures should establish what was found. When autonomous and expert-guided conditions exist, identify their separate outputs and what intervention changed. Keep benchmark scores, execution status and task counts in their evidentiary roles; do not invent such experimental arms elsewhere.

8. **Show authentic comparison examples.** When evaluating visualization or interpretation quality, include actual generated outputs where available, identify their origin, and explain input/task differences. Select examples through a defensible rule. Scores alone may leave the claimed advantage invisible; an attractive example alone does not establish general superiority.

## Visual grammar and prototypes

9. **Prototype consequential designs.** Inspect representative real panels before extending a new visual approach across the set. Compare useful alternatives when communication is uncertain. Follow the selected mode for human review; routine reuse of an accepted design needs no extra approval ritual.

10. **Study appropriate reference designs.** For unfamiliar scientific structures, examine relevant primary publications and specialist plotting examples. Adapt the visual logic to the actual evidence. A particular library, paper palette or graph layout remains a task-specific choice rather than a universal requirement.

11. **Build comparable geometry.** Use aligned baselines, consistent row order, common units and shared scales for comparable quantities. Explain necessary transformations or scale differences. Related graph panels should preserve category colours and comparable degree-to-size mappings. Annotated and clean variants should differ only as requested, preserving underlying data and geometry. Verify comparable panels using [final rendered plot areas](figure-verification.md#final-render-geometry), not source layout settings alone.

12. **Give channels explicit meanings.** Position, colour, size, shape and line style must have defined roles and agree with the legend. Choose categorical, sequential or diverging palettes appropriately. Preserve category meanings across related figures; avoid using colour or size to imply an unsupported quantitative order.

13. **Follow the visual profile.** Match established manuscript typography, palette, panel-letter convention and annotation style, subject to the target venue. Maintain contrast and controlled saturation. Configure fonts, including any author-preferred family, in the project profile; do not impose a historical font, palette or black-text preference on every manuscript.

14. **Add interpretable reference marks.** Show relevant zero lines, thresholds, null bands and known-answer anchors with visual weight below the data. Explain uncertainty when it affects interpretation. Do not invent controls, repeats or intervals to satisfy a template. A shaded confidence band is data encoding, not decorative background. For inferential comparisons in the artwork or caption, apply the shared [statistical reporting checks](../../manuscript-audit/references/statistical-reporting.md) at that scope.

15. **Balance density and readability.** Use white space to group evidence, protect labels and guide reading. Recompose sparse figures and facet crowded ones. Label interpretation-changing exceptions rather than every point. Apparent all-zero or identical outcomes require source/renderer checks; scientifically meaningful negative findings remain available.

16. **Design networks scientifically.** Define node/edge classes, subset eligibility, selection rules and group labels. Preserve the difference between data-derived communities and hypothesized biological categories. Balance node and edge visibility so relationships can be read without a hairball or disconnected-looking cloud. A community partition does not validate a functional class.

## Composition, provenance and delivery

17. **Keep quantitative plates focused.** Exclude decorative boxes, tinted backgrounds, text-only filler and unnecessary flowcharts. Permit scientifically necessary architecture schematics, actual task graphs, authentic image plates and data-encoded bands. Put figure and panel headings in the legend; retain necessary axes, panel letters, direct labels and encoding keys.

18. **Assemble without distortion.** Preserve aspect ratios, align panel letters near the upper left, and maintain consistent spacing and scale. Reflow after removing headers. Split oversized composites by coherent subquestion instead of severely compressing them. Final placement, including width and height constraints, determines legibility; inspect that geometry explicitly.

19. **Render scientific plots with suitable tools.** Prefer reproducible plotting code for quantitative figures and appropriate vector tools for diagrams. Keep a review gallery separate from the scientific artifact. Choose tools for the output rather than mandating one language or assembly system; avoid manual transcription of numerical marks. For Python/Matplotlib manuscript plots, read [figures4papers.md](figures4papers.md) for reusable patterns and implementation conventions; retain this workflow's evidence, visual-profile and review requirements.

20. **Reuse sound existing work.** Inspect available plotting code, sources and intermediate panels before replacing them. Preserve correct scientific transformations while improving presentation. Missing historical code is an evidence limitation; do not fabricate a new script and present it as the original method.

21. **Retain the plotted evidence.** Preserve source identifiers, filters, aggregation/ranking rules, exact plotted-object data where appropriate, plotting code, panels and assembly. Use stable scientific sources rather than mutable numbered-figure folders as the sole input identity. Explain unavailable provenance instead of silently substituting a similar dataset. For microscopy, gels, blots and related image evidence, keep the applicable [image-processing and calibration record](figure-verification.md#image-integrity-record).

22. **Preserve evaluated originals.** When the claim concerns what a participant or agent generated, keep the scored image identifiable and unchanged. A restyled derivative may explain the analysis, with its origin disclosed, but cannot replace the evaluated artifact or inherit its score without an appropriate new evaluation.

23. **Export genuine suitable formats.** Preserve vector text and paths where useful; retain legitimate raster evidence at adequate resolution for final size. Produce inspectable previews. A PDF/SVG extension does not make embedded raster panels vector. Verify fonts, glyphs, crop, transparency and actual output properties rather than assuming export success establishes them. Keep [collision findings tied to the current export](figure-verification.md#current-export-collision-check), including after revisions that change text or mark geometry.

24. **Maintain one traceable active set.** Distinguish final, temporary, alternative and archived assets with recognizable mappings. Do not clone final panels over historical alternatives. Keep scientific-purpose/legend notes and source material accessible when organising a substantial set. Apply cleanup only within authorization and preserve concurrent or unrelated work.


## Nature Communications artwork quality baseline

The author's standing preference is that every main and supplementary manuscript figure receive the care expected of Nature Communications or a more selective research journal. Treat this as an artwork and evidence-communication baseline, not a claim of journal endorsement, acceptance, or scientific significance. Apply the same standard in Easy mode.

- When the author supplies a concrete figure-quality reference, inspect its actual figure plates and available plotting sources before redesigning. Compare the breadth of evidence, panel roles, alignment and reading order, not only colours, typography or resolution. Retrieve relevant unused patient-, sample-, feature-, fold- or condition-level evidence from the project to replace sparse headline-only summaries. Build a coherent result aspect across complementary panels, such as primary observations, full comparison matrices, distributions, uncertainty and robustness. Do not copy the reference's scientific content, impose a fixed panel quota or add redundant panels to simulate richness. Keep the particular reference path and figure mappings in the project record.
- For every figure, inspect the actual source data and existing artwork, write a concise panel purpose and comparison plan, and deliberately compose the figure. Do not deliver a repeated default two-panel template, oversized empty axes, isolated trivial plots, or a resolution-only upgrade in response to a quality complaint. Use a compact shared-row or shared-scale comparison where it reveals the result; preserve sufficient breathing room and legibility.
- Consult the current [Nature research figure guide](https://research-figure-guide.nature.com/figures/preparing-figures-our-specifications/) and the actual target journal's artwork instructions. Record project-specific final dimensions, font sizes, line weights and export settings. Preserve the manuscript's accepted typography and target venue when adopting Nature-style artwork. Do not silently switch journals or document templates.
- Require clear visual hierarchy, aligned panel geometry, consistent semantic colours, colour-vision-accessible encodings, readable black labels, defined units and unobtrusive reference marks. Use redundant shapes or positions where colour alone is insufficient. Quantitative panels should expose the relevant comparisons, distributions or relationships; avoid decorative complexity and unsupported biological diagrams.
- Preserve observations, denominators, transformations, censoring, missingness, effect direction and uncertainty definitions. Label SD, confidence intervals, bootstrap intervals and simulation variability distinctly. Keep null findings visible. Never add artificial observations, confidence bands, significance marks or extra experiments to make a figure appear more sophisticated.
- Export genuine editable vector PDF/SVG with live text and embedded fonts where applicable. High-resolution raster files are derivatives; increasing DPI or wrapping a bitmap in a PDF does not meet the baseline. Preserve reproducible plotting code and the exact plotted data. Keep superseded artwork identifiable in its project archive.
- Inspect **every** individual main and supplementary figure at final publication size and inspect its actual manuscript placement. Check label collisions, clipping, panel letters, font/glyph embedding, colour accessibility, caption agreement and source fidelity separately. Iterate until concrete defects are resolved. A contact sheet, file count, numerical score or successful export alone is not acceptance evidence.
- Replace the active figures, manuscript insertions, legends, supplementary files and delivery archives consistently. Save deliverables in the manuscript's own project folder. Report the checks actually performed and any remaining limitations; do not certify an “NC-level” scientific contribution from visual inspection.

## Deliverable and acceptance

A substantial figure task yields a concise panel plan, finished artwork, necessary panel exports, complete legend, sufficient source/transformation material for new quantitative claims, and a proportionate verification record. A small authorized restyle need not create extra scaffolding.

Legends decode every necessary line, point type, colour, shape, size scale and reference mark, with conditions, units, sample/aggregation units and applicable centre/spread/uncertainty definitions. Remove internal revision tags and working-caption notes. Keep scientific model/database versions visible where needed to interpret conditions, with full Methods detail.

Inspect individual exports, assembled figures and actual manuscript insertions. Report data fidelity, readability, caption alignment and export/package verification separately. Journal-specific numerical font, canvas and resolution requirements belong in the current visual profile; historical thresholds are not universal gates.
