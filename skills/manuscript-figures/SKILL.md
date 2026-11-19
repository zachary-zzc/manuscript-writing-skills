---
name: "manuscript-figures"
description: "Plan, create or revise scientific manuscript figures, panels, tables and captions, including reproducible static plots. Use for manuscript artwork and display legends; exclude interactive Crux bundles and unrelated visualizations."
---

# Manuscript Figures

Read the [shared manuscript contract](../manuscript-workflow/references/contract.md) first. Reuse the task's confirmed Easy, Normal or Expert mode, scientific storyline, evidence and visual profile. This skill does not restart intake or introduce another review mode.

## Hard rules for manuscript narrative

Apply the **Editorial Guideline (mandatory default)** in [release narrative and defensive-writing rules](../manuscript-workflow/references/release-narrative-rules.md) before drafting, restructuring, polishing, auditing, or reviewing. They are hard defaults, with special priority for manuscript writing, storyline, idea framing, and innovation claims. When the user supplies manuscript text, perform the required point-by-point defensive-writing audit and give a concrete rewrite for every instance. Preserve material limitations, negative findings, uncertainty, ethics, safety, and reproducibility boundaries as precise evidence or scope statements.

For Nature or Nature Portfolio targets, follow the [canonical Nature integration map](../manuscript-workflow/references/nature-integration.md) and load only the relevant `nature-shared` reference; this manuscript skill remains the owner.

Load only the guidance needed for the requested display work:

- For figure-set planning, new artwork or a substantive redesign, read [scientific figure generation](references/figures.md). Preserve the source evidence, evaluated originals, accepted typography and actual target venue.
  Also read [visual form selection and main-figure composition](references/visual-form-selection.md). For every new or redesigned main figure, document the data structure, panel duties, chosen form, rejected alternative and anti-default check.
- For Python/Matplotlib manuscript plotting, also read [figures4papers patterns](references/figures4papers.md). Keep its attribution and license notice. This is an implementation reference, not an importable plotting package; existing R and vector workflows remain valid.
- For comparable multi-panel layouts, revisions that change text or mark geometry, schematics, or microscopy/gel image panels, read the applicable sections of [figure verification](references/figure-verification.md). Keep measured checks distinct from visual inspection and checks not assessed.
- For captions, legends or scientific tables, read [captions and tables](references/captions-tables.md). A bounded caption edit needs the affected display, source facts and narrative checks; it does not require a new storyboard or redesign of the figure set.
- For generated or redesigned artwork, apply the [four visualization audit layers](../manuscript-audit/references/audit.md#four-independent-visualization-audit-layers) to the affected displays. Load further audit guidance only when the requested scope requires it.
- For placement or typesetting requests such as loose pages, stranded headings, oversized floats or sparse Supplementary Information, read [LaTeX layout and float typesetting](references/latex-layout.md). Render and inspect the compiled pages before and after changes.

Make consequential design decisions reviewable with actual evidence and representative artwork under the shared mode. Preserve accepted designs during local revisions. Deliver the requested artwork or caption, relevant source and export material, and the checks actually performed. Keep unsupported source facts explicit rather than inventing data or uncertainty.

Keep quantitative plots in reproducible local Python/R or equivalent source code. `image_gen` may assist with non-data illustrations or schematic assets, but never with quantitative evidence. If a connected Figma or diagram tool is used, treat it as optional vector/layout assistance only; keep the data, plotting code and final scientific QA in the manuscript project.
