# Manuscript and visualization audit

Use for requested audits and checks justified by the edit. A paragraph polish needs targeted verification; it does not automatically trigger a complete forensic audit or independent peer-review exercise. An audit-only request remains read-only. Follow the confirmed mode for consequential decisions and preserve the authorized scope.

## Whole-manuscript structure and paragraph audit

Before a full-manuscript audit or full/substantive manuscript revision, inspect the entire current manuscript and its supporting material. Complete this diagnostic before rewriting; preserve accepted decisions and distinguish new findings from issues already resolved. Explicitly bounded local wording, paragraph/section polishing or layout work uses targeted checks unless a change in meaning requires broader reconciliation. Do not turn a typo correction into an unrelated forensic audit.

1. **Structure and storyline first.** Map the scientific question, motivating gap, central contribution, evidence dependencies, section/subsection roles, transitions and conclusion. Test the complete argument against the actual evidence before polishing its language.
2. **Read the entire manuscript in this audit order:** Introduction → Abstract → Results → Methods, followed by Discussion and every other section present. This is a diagnostic reading order for the audit only. Production order remains H0 → H1–H4 → H5–H6 → H7 Results and figure iteration → H8–H11. Inspect each subsection and each paragraph in sequence. Also cover the title, headings, tables, figure panels and captions, references, declarations and Supplementary Information. Consult dependent evidence whenever needed and reconcile the abstract/title again after the complete pass.
3. **Keep a coverage ledger and audit continuity.** Give every paragraph or other review unit a stable location/ID. Apply the [terminology and logical-continuity procedure](../../manuscript-workflow/references/paragraph-review.md#terminology-and-logical-continuity), recording substantive checks, outcomes, linked findings and repairs in the same ledger. Account explicitly for every subsection and supporting unit. Do not substitute selected examples, paragraph sampling, or a blanket section-level pass for the complete read. Mark inaccessible material and unresolved facts as gaps rather than passed.
4. **Reconcile the complete paper.** Apply the [cross-document consistency checks](#cross-document-and-source-consistency) to the terminology decisions, logical repairs and evidence findings. Record conflicts and every dependent location that a repair must address.
5. **Report the integrated judgment.** Separate structural/storyline findings, paragraph- and sentence-level findings, global consistency findings and evidence gaps. State the coverage achieved and material remaining dependencies. A thorough read does not by itself establish numerical reproduction, figure verification or submission readiness; report those checks separately.

This audit depth applies in Easy, Normal and Expert. The mode controls human review checkpoints, not terminology, paragraph or sentence checking standards. Audit-only requests produce findings and concrete revision proposals without automatically editing the manuscript, changing raw records or launching experiments.

## Multi-pass manuscript audit

Run the following passes for every new or substantially revised full manuscript. Record each pass separately in the existing audit ledger and rerun affected passes after any material change.

1. **Architecture and evidence pass** after H1–H4. Check the framework record, question, contribution, drawback map, Results order, claim boundaries, evidence dependencies and complete terminology table. Record its version and unresolved entries.
2. **Results–figure pass** after H7 and every figure iteration. Check numerical reproduction, source fidelity, denominators, conditions, panel geometry, encodings, captions, callouts, final-size readability and the four independent visual layers.
3. **Supplementary Information pass** after H9S. Check the SI inventory and outline, supporting analyses, protocols, source data, supplementary figures/tables, captions, references, assets, main-text callouts, numbering, cross-references and compiled SI pages. Apply the same visual audit to every supplementary display and reject orphan, duplicate or unsupported items.
4. **Cross-section language pass** after H8–H11. Check terminology, abbreviations, claim strength, transitions, citations, defensive language, uncertainty, limitations, negative findings, ethics, safety and reproducibility boundaries across every section, SI item and display.
5. **Integrated package pass** at H12. Compile main text and SI, inspect actual pages and figures, resolve citations and numbering, verify references, freeze the terminology table against the rendered package, check layout and package dependencies, then rerun the terminology and defensive-language checks on the final rendered version.

A pass is **passed**, **failed**, **not assessed** or **requires author input**. “Not assessed” is never equivalent to passed. The final package is complete only when all applicable pass results are passed or carry an explicit unresolved status reported to the author.

## Terminology and logical continuity

Apply the canonical [paragraph and sentence review](../../manuscript-workflow/references/paragraph-review.md#terminology-and-logical-continuity), including its terminology table, paragraph reverse outline and sentence-by-sentence checks, at the scope established above.

## Scope, evidence and findings

Identify the authoritative source/version, target, supplied materials, excluded evidence and protected content. Inspect relevant sources before judging claims. Check external audit findings against this version and classify them as confirmed, resolved, unsupported or unresolved. Verify proposed replacements as carefully as the original wording; a reviewer's recommendation is not evidence of correctness. A gap in a bounded packet does not prove absence from the study. Recheck historical findings against later resolutions; neither a memory nor an author clarification alone establishes artifact-level verification.

Maintain claim-to-evidence links for substantive background assertions and motivating drawbacks as well as headline and method-dependent claims: location, exact source or artifact, condition/population, calculation where applicable, uncertainty and permitted interpretation. Check that each citation supports the asserted characteristic and consequence at the stated scope; a related paper or a record of heterogeneous data alone does not establish the claimed problem. Mark the distinction between a cited finding and an author inference in the existing review record. Record actionable findings with an ID, severity/status, source or screenshot, check/result, scientific consequence, repair and pass condition. Distinguish confirmed error, aggregation ambiguity, provenance gap, suspected duplication, unresolved author input, not assessable and passed. Severity follows scientific impact, not the number of characters changed.

Check evidence levels separately: registered capability, planned work, invocation, successful retained output and validated conclusion. A report naming a tool or API does not prove execution. Inspect relevant commands/calls, logs, exit status, outputs and implementation. A local snapshot differs from live retrieval; deposited code differs from an independently developed method; checkpoint inference differs from training. Do not substitute current scripts/defaults for historical configurations or let a later extension validate earlier runs.

Preserve original questionnaires, labels, raw independent ratings, reviewer reports and evaluated images. Add analytical crosswalks or correction notes separately. Correct data only within appropriate authorization: preserve originals, identify affected records and dependent fields, document the basis, recompute derived results and propagate consequences. Audit permission alone does not authorize changing raw ratings or launching experiments.

## Numerical, statistical and comparative checks

When statistical analyses or inferential claims are in scope, also apply the focused [statistical reporting checks](statistical-reporting.md). The unit, multiplicity and comparison rules below remain canonical; the reference adds reporting and interpretation checks without duplicating them.

- Recompute central totals, percentages, differences, ratios, weighted summaries, rounding and integer constraints. Record source, expected/recomputed value, convention/tolerance and outcome. Undefined aggregation remains ambiguity until resolved.
- Attach each important numerical claim to its measured object, metric definition, comparison condition and relevant aggregation. Define formula, units, scale/direction, positive class, denominator, weighting and zero/empty handling as applicable. Distinguish percentage points from relative percentages and unique entities from overlapping annotation counts. Metrics expressed on the same percentage or score scale can measure different outcomes; do not substitute one for another merely because it is easier to describe.
- Identify independent and dependence units. Repeated ratings, objective-condition cells and genome pairs sharing members are not independent replicates. Match pairing, clustering, bootstrap and permutation units to the design.
- Preserve complete multiplicity families and eligibility rules. Displaying selected significant clusters does not authorize correcting only that displayed subset. Verify P/q values, exclusions and sensitivity analyses.
- Define error bars and interval estimands. Overlap alone determines neither significance nor equivalence; non-significance does not establish equivalence. A point above a null median is not a permutation P value.
- Check common objectives, inputs, resources, model/configuration identity, evaluator coverage and validation designs. Describe unmatched comparisons honestly. Workflow tiers do not isolate causal component effects. Human and automated contrasts with different cohorts, condition families or weighting are complementary evidence, not interchangeable effect sizes.
- Keep heterogeneous endpoints in their own units. An aggregate score needs a justified estimand and documented contract. A tolerance-based recovery count needs endpoint definitions and prespecified/retrospective status; avoid calling it exact agreement.
- Separate frozen-output recomputation from repeated new execution. A historical run supports its retained result without estimating repeatable success rates. Numerical reproducibility need not require identical hosted-model trajectories.
- Bound interpretation: annotation, prediction, association, candidate, function and mechanism are distinct. Examine source composition, missingness and subgroup reversals. Top-ranked retained features do not reconstruct full-model importance; model use does not establish biological mechanism.

## Four independent visualization audit layers

Report **passed**, **failed**, **not assessed** or **requires author input** for each applicable layer. A pass in one cannot establish another. Inspect every panel in scope; do not credit a claimed property without source evidence or visible output.

### A. Scientific and data fidelity

Identify actual panel versions and claims. Reconcile values, cohorts, conditions, unique entities, exclusions, denominators, units, category labels and summary definitions. Trace visible marks and annotations to source rows or defining statistics. Scatter points require paired observations; boxplots require observations or complete defining statistics. Never manufacture individual values from means.

For schematics or microscopy/gel image evidence, apply the matching [component/edge and image-integrity checks](../../manuscript-figures/references/figure-verification.md#schematic-components-and-edges), without invoking an unrelated figure-production workflow.

Inspect rankings against all eligible records, including direction and ties. Validate Boolean/class mappings and distinguish zero, unknown, missing and excluded categories. Check axis direction/limits, transforms, conversions and common-scale compression. Colour or side-by-side placement does not create a separate quantitative axis. Disclose plot-induced omissions such as log-excluded zeros, clipped outliers and hidden categories when they affect interpretation.

Verify uncertainty, resampling units, multiplicity families, statistical labels and thresholds. Investigate empty or identical-looking outcomes through source values, filtering, scale, clipping and renderer behavior. Retain important null results. Pass only when the measurement objects, calculations, populations and claims match retained evidence; missing sources remain explicit gaps.

### B. Readability and composition

Inspect pixels from individual exports, assembly and final manuscript placement. Account for width reduction, height clamps and oversized export canvases. Read ticks, axes, legends, colorbars, annotations and scientific symbols at intended size. Font floors, canvas dimensions and DPI targets are configurable venue/output requirements.

Check text-text, text-mark, legend-mark and neighboring-panel collisions; clipping, lost glyphs, cropped data and truncated colorbars; aspect ratio, panel spacing and consistent upper-left letters. Inspect adjacent panels after finding a collision. Recompose oversized plates rather than forcing unreadable reduction.

For comparable panels and collision verification, use the figure owner's [final-render geometry and current-export checks](../../manuscript-figures/references/figure-verification.md#final-render-geometry). Separate measured alignment, visual inspection and automated findings; an earlier report does not verify a changed export.

Check purpose, distinct evidentiary roles, redundancy, whitespace and clutter. Apply the established palette and category semantics. Require adequate contrast and non-colour cues where hue alone obscures necessary distinctions; red/green hue alone is not colourblind-safe. A valid two-point comparison or authentic image does not fail an arbitrary minimum-mark heuristic. Pass when readers can read and identify the evidence without misleading geometry or unexplained channels.

### C. Legend, narrative and interpretation

Compare visible content with the caption, source table, Methods and Results. Pixels establish what is drawn; prose cannot create an absent axis/distribution or turn impurity importance into SHAP. Legends explain necessary panels/encodings, conditions, units, n and applicable centre/spread, whisker, point and uncertainty definitions. Body prose does not repair a missing caption definition.

Verify meaningful main/SI display and panel callouts, first-appearance order and actual compiled numbering. Use scientific content and stable labels rather than filename numbering. SI should extend evidence, avoiding unnecessary main-panel duplication. Remove working notes, stale artwork tags and engineering residue; retain scientific versions wherever needed for comparison. Pass when readers can interpret the visible evidence and the narrative preserves its actual scope.

### D. Export, provenance and package

Inspect real vector/raster content, final-size resolution, fonts, glyphs, crop boxes and transparency. File extensions prove none of these. Bind source, script, panels, assembly and active manuscript asset; check recognizable final/alternative mappings. Preserve scored originals and requested clean/annotated identity.

Compile actual main/SI sources and inspect their output for intended versions, page fit, blank panels/pages, panel letters and caption placement. Distinguish code inspection, rerendering, pixel inspection and numerical reproduction. Pass only for supplied/inspected properties and the package's claimed reproducibility; do not infer a functioning historical script from an existing image.

## Cross-document and source consistency

Reconcile terminology and abbreviations, concepts and definitions, storyline and claim strength, populations and sample units, endpoints and time origins, methods and comparison conditions, numbers and uncertainty, citations and display callouts, and main/SI correspondence. Search both repeated wording and related meanings. The same term must retain its definition, and distinct concepts must not be collapsed for stylistic variety.

Propagate changed meaning across Title, Abstract, Introduction, Results, Discussion, Methods, captions, tables, SI, availability and submission materials in scope, including text embedded in artwork. A denominator change affects rates and deviations; a protocol change can invalidate “independent,” “same inputs,” “prespecified” or “reproduced.” Check that shortened descriptions preserve meaning, resource versions remain distinguishable from experimental datasets, and hypotheses, candidates and established findings retain their evidence level. Reapply the paragraph and sentence continuity checks around substantive edits, including neighbouring transitions; a repaired passage must not leave a contradictory claim elsewhere.

Check exact citation support and source identity; use primary evidence for technical capability and novelty claims. Preserve relevant method credit during compression. Inspect included sources and compiled references for missing/duplicate labels, unresolved citations, bibliography keys, callouts and numbering. Verify promised conservation of protected sections, equations, numbers, citations or artwork through appropriate comparisons; correction tasks can legitimately change numerical values.

For substantive citation-support checks, literature discovery or bibliographic corrections, use the shared [literature procedures](../../manuscript-workflow/references/literature.md). A formatting-only citation edit does not require a new literature search.

When data/code access is part of the requested declaration or submission-package audit, use [data availability and reuse](data-availability.md) to reconcile statements with the actual records and access conditions. A bounded statement edit checks the affected datasets and claims, not the entire study's deposit readiness.

## Independent review and completion

Use independent mock peer review when requested or warranted by scope, without automatically requiring three reviewers. Give reviewers the same frozen packet and applicable criteria with complementary emphases. Keep contexts genuinely isolated, freeze reports before synthesis/forensic follow-up, and preserve disagreement and important single-reviewer findings. Later arithmetic discoveries are audit findings, not retrospective independent consensus. Review judgments are not journal decisions.

Resolve findings through retained-evidence reconciliation, authorized reanalysis, correction, documentation or claim narrowing. Identify missing evidence without automatically commissioning new studies. Keep original records and append resolution status; never invent historical settings, methods, declarations or access links.

After authorized edits, rerun affected checks. Use a real compiler and inspect diagnostics, unresolved references, overflow and float problems. Render PDFs and inspect affected pages at readable scale; use whole-document contact sheets when scope warrants. Check typography, cropping, proportions, tables, headings, captions and column gaps. Fix the layout cause rather than distorting figures or scattering forced breaks. If compilation/rendering is unavailable, report that verification gap.

Deliver usable sources with required bibliography, styles, images and working dependencies. Report prose completion, evidence reconciliation, numerical reproduction, scientific support, four visual layers, compilation, inspected layout, package completeness and current venue compliance separately. Successful compilation is not scientific validity or submission readiness; external submission retains its own authorization.
