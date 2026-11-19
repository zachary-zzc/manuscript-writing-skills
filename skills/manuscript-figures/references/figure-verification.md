# Figure verification for rendered geometry and scientific meaning

Use only the sections relevant to the affected artwork. These checks supplement the [four visualization audit layers](../../manuscript-audit/references/audit.md#four-independent-visualization-audit-layers); they do not replace source verification or final-size visual inspection. Keep the established mode, visual profile, accepted design and protected originals. Use available rendering and inspection tools without requiring a particular backend, imported audit script or new dependency. Record findings in the existing figure QA record rather than creating a parallel review workflow.

This reference adapts selected Nature-skills guidance; see the [integration source record](../../manuscript-workflow/references/nature-integration.md) for attribution and boundaries.

## Final-render geometry

Apply this check when two or more panels invite geometric comparison. Define the relevant row/column groups and intended shared edges, dimensions or spacing. A single panel has no inter-panel alignment requirement; intentionally unrelated panels need not share dimensions.

- Measure actual plot-area rectangles after the final layout has resolved fonts, legends, colorbars and export dimensions. Use the renderer's final geometry or a calibrated measurement of the export. Source grid settings alone do not prove rendered alignment. Use plot areas for axes alignment and outer-content bounds for clearance; unequal tick-label widths do not necessarily mean shifted data areas.
- Record final physical size, measurement method, comparison groups, measured deviations and the applicable tolerance in the figure QA record or a small machine-readable table. Use the project's visual profile or a justified tolerance for this output; no numerical threshold is universal.
- Check relevant shared edges, comparable widths/heights, repeated gutters and panel-letter anchors. In unequal-span layouts, compare shared outer boundaries without requiring a spanning panel to match a smaller panel's height. Distinguish insets, colorbars and legend-only regions from data panels. Record an intentional exception for the affected panel and check, with its reason; do not relax every comparison to hide one exception.
- Remeasure affected groups after geometry-changing revisions. If geometry cannot be measured reliably, mark the measurement **not assessed**, state the limitation and report any visual inspection separately. Do not turn plausible-looking alignment into a measured pass.

## Current-export collision check

Inspect the final exported artwork at its intended size. Tie the record to the exact export/version, physical dimensions and inspected panels; a content hash is useful when available. State whether findings come from visual inspection, measured geometry or an automated detector. Do not label a manual inspection as an automated pass.

Check text against other text, lines, markers, error bars, image/fill boundaries, neighboring panels and page edges. Use the full uncertainty extent when assessing label clearance. Distinguish obscured data or clipped text from intentional, legible labels contained inside bars, heatmap cells or images. Interpret detector findings against the actual figure and document accepted overlays; geometry alone cannot establish adequate contrast, scientific correctness or readability.

Changes to text, fonts, data/mark geometry, uncertainty, legends, annotations, panel dimensions or placement invalidate the affected earlier findings. Re-export and inspect the changed artwork and relevant neighboring panels; rerun an automated check if its result is being reported. Repair real conflicts by moving labels or recomposing the layout, not by hiding data lines or uncertainty with opaque masks. Keep any diagnostic overlay separate from submission artwork. If a detector or measurement is unavailable, mark that check **not assessed** and retain the scope and result of any manual review.

## Schematic components and edges

Treat a component, connection and arrow direction as claims. For each component and scientifically meaningful edge, identify support in the study's code, configuration, Methods or other authoritative evidence. Record its endpoints, direction where applicable, what moves or what relationship is asserted, and the conditions under which it exists, including optional paths or experimental arms.

Distinguish data transfer, control, feedback, experimental steps, association and causal claims where present. Give each line style one defined meaning within the figure and preserve it in the caption. Check that connectors end on the intended object rather than accidentally implying a connection to its whole container. Draw loops, fixed sequences and tool calls only when the actual system supports them; an agent label alone does not establish iterative behavior. Resolve unsupported boxes or edges by narrowing or removing the claim within the authorized scope, or record the missing source. Do not invent a mechanism to complete a diagram.

## Image-integrity record

For actual microscopy, gel, blot or related image evidence, retain the applicable record:

| Item | Record |
|---|---|
| Provenance | Raw and processed source identities, panel mapping and available processing history |
| Processing | Crop, brightness/contrast/gamma, pseudo-colour and other transformations actually applied |
| Composition | Stitching or lane rearrangement, source boundaries and reuse in other panels |
| Calibration | Physical scale and its source, with a calibrated scale bar where spatial dimensions are interpreted |
| Quantification | Link from the displayed image to the associated measurement or analysis |

Mark unknown history as unknown; do not reconstruct it from an attractive final image. Check whether processing hides relevant background, bands or features, even when the adjustment is global. Preserve originals and apply the target venue's disclosure requirements. A magnification label alone does not establish the scale after resizing; verify calibration against the displayed asset. These records do not authorize altering raw images or replacing evaluated originals.
