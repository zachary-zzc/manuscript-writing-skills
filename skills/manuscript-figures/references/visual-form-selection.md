# Visual form selection and main-figure composition

Use this reference for every new or substantially redesigned main figure or figure set. It is a decision aid, not a fixed style template. Choose the visual form from the scientific question and data structure before choosing colours, templates or a plotting library. Preserve source fidelity, uncertainty, denominators and required comparisons. Visual variety never justifies unsupported transformations or cherry-picking.

## Required design sequence

1. State the reader question, central claim and panel duty in one sentence.
2. Classify the evidence structure before selecting a chart: ranking, distribution, paired or repeated observations, trajectory, relationship, composition, matrix, hierarchy, network or flow, spatial pattern, image evidence, mechanism, or multi-metric comparison.
3. Name the candidate encoding and at least one credible alternative whenever the choice is not obvious. Record what the chosen form reveals, what the rejected form would hide, and why the choice fits the evidence.
4. For a main figure, storyboard the smallest coherent set of complementary roles needed for the claim, such as context, primary observation, principal comparison, mechanism or structure, and robustness or boundary. Use only the roles the evidence supports.
5. Inspect the rendered figure at final publication size, in grayscale or a colour-vision-accessible simulation when colour carries meaning, and at its actual manuscript placement.

## Data structure to visual form

| Evidence structure or reader question | Strong candidates | Inspect before accepting |
|---|---|---|
| Ranking across a small set of entities | Sorted dot or interval plot; bars when a common zero and magnitude comparison are central | Whether ordering, uncertainty and denominators remain visible; lollipop is acceptable only when its sparse baseline adds meaning |
| Distribution across groups | Raw points with jitter or beeswarm, violin or density, raincloud, or an interval plus raw observations | Sample size, tails, multimodality, overplotting and whether a box summary hides the distribution |
| Paired or repeated measurements | Paired points, slopegraph, within-unit trajectories, or small multiples | Whether aggregation erases pairing, crossover, heterogeneity or missing visits |
| Ordered time or dose trajectory | Lines with points, ribbons, event annotations, or phase-specific small multiples | Whether the x-axis is truly ordered, lines imply unsupported continuity, or too many series create spaghetti |
| Relationship between variables | Scatter, density, hexbin, contour, or small multiples | Overplotting, marginal distributions, transformations, and whether a fitted line is justified |
| Composition or part-to-whole | Stacked bars or areas, 100% composition, ternary plot for three constrained parts, or alluvial for supported flows | Whether segment comparisons are readable and whether the visual implies a flow or conservation that was not measured |
| Matrix or pairwise structure | Heatmap, clustered heatmap, correlogram, or aligned small multiples | Ordering rule, missing cells, scale direction, clustering provenance and whether colour is doing too much work |
| Hierarchy or nested categories | Dendrogram, treemap or sunburst when the hierarchy is real and central | Whether area and nesting remain interpretable and whether the hierarchy is data-derived rather than invented |
| Network or flow | Network, arc, chord or Sankey only when relationships and direction are supported | Node and edge eligibility, hairballs, edge semantics and whether a simpler matrix or adjacency view is clearer |
| Spatial or geographic evidence | Map, choropleth, dot density, spatial point map or faceted map | Projection, denominator, spatial aggregation, uncertainty and whether colour implies a continuous field |
| Image, microscopy, gel or structural evidence | Authentic image panels, calibrated crops, overlays or aligned image grids | Provenance, scale bars, processing history, calibration and whether annotations obscure evidence |
| Mechanism, pipeline or experimental design | Evidence-supported vector schematic, process diagram or actual task graph | Every box, edge, arrow direction and loop; remove unsupported causal or control claims |
| Several metrics or conditions | Aligned small multiples, heatmap, parallel coordinates or a radar chart only for a small set of commensurate metrics | Shared scale, metric direction, missing values and whether radar geometry hides the comparison |

The table does not require a different chart for every panel. Reuse a form when a shared geometry makes comparisons faster. Do not reuse it because a template is convenient.

## Anti-default gate

Before accepting a repeated line-point, bar, lollipop, radar or single-summary panel, answer:

- What scientific structure does this form reveal?
- What structure would a raw-point, distribution, paired, interval, matrix or small-multiple alternative reveal instead?
- Is the chosen form selected because of the claim, or because it was the first available plotting template?
- Does the main figure make the central result visible without forcing the reader to infer it from a table or legend?
- Do panel forms differ because their evidentiary roles differ, while typography, semantic colours, scales and reading order still make the set coherent?

If every panel uses the same form, document why comparability requires it and check whether at least one panel would communicate its structure better with another form. If a lollipop or radar chart is used, record the specific reason it is preferable to a sorted interval plot or aligned small multiples.

## Main-figure aesthetic audit

Assess visual hierarchy, whitespace, label density, panel rhythm, semantic colour consistency, contrast, accessible encodings, direct annotation, and final-size legibility separately from data fidelity. Reject decorative complexity, empty axes, repeated filler panels, unsupported icons, and default layouts that leave the central finding visually secondary. A strong main figure should read in a deliberate order, show the strongest supported result first, and use later panels to explain comparison, mechanism, boundary or robustness rather than repeat the same mark type.

## Reference decision aids

- [Nature figure specifications](https://research-figure-guide.nature.com/figures/preparing-figures-our-specifications/) for current production constraints and artwork checks.
- [A checklist for designing and improving the visualization of scientific data](https://www.nature.com/articles/s41556-025-01684-z), Nature Cell Biology (2025), for clarity, accessibility and design principles.
- [From Data to Viz](https://www.data-to-viz.com/) for a data-format decision tree and chart-specific caveats. Use it as a design aid, not as a substitute for study-specific evidence or statistical judgment.
- [Fundamentals of Data Visualization](https://clauswilke.com/dataviz/) for perceptual and compositional explanations of common forms.
