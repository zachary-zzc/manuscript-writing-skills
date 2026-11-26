---
name: manuscript-workflow
description: "Manage a scientific manuscript workflow: identify its current state, decide the next step, resume ongoing work, and coordinate section skills, reviews, revisions and final assembly. Use for whole-paper work, cross-section changes, journal-specific manuscript targets including Nature Portfolio titles, or manuscript-specific requests such as what next, where are we and continue. Use the matching section skill directly for a bounded section task; skill maintenance needs no manuscript mode."
---

# Manuscript workflow manager

## Hard rules for manuscript narrative

Apply the **Editorial Guideline (mandatory default)** in [release narrative and defensive-writing rules](references/release-narrative-rules.md) before coordinating or reviewing manuscript work. They are hard defaults, with special priority for manuscript writing, storyline, idea framing, and innovation claims. When the user supplies manuscript text, perform the required point-by-point defensive-writing audit and give a concrete rewrite for every instance. Preserve material limitations, negative findings, uncertainty, ethics, safety, and reproducibility boundaries as precise evidence or scope statements.

Read the [shared contract](references/contract.md) once for the continuing task. Keep one accepted storyline, evidence boundary, terminology record and Easy/Normal/Expert mode across specialists. Load only the skill needed for the current work; do not preload every section or make a specialist invoke this coordinator again.

## Canonical journal routing

The `manuscript-*` suite is the single authoring and editing system for every journal target, including Nature and Nature Portfolio titles. Do not start a parallel Nature writing or polishing workflow. Keep the same section owner, interaction mode, evidence boundary and accepted decisions; add journal-specific guidance only when the target or request requires it.

- Whole-manuscript narrative or Introduction: load [`nature-introduction.md`](../nature-shared/core/nature-introduction.md).
- Abstract: load [`nature-abstract.md`](../nature-shared/core/nature-abstract.md).
- Results or Discussion: load [`nature-results-discussion.md`](../nature-shared/core/nature-results-discussion.md) and, for Discussion argument functions, [`discussion-argument-language.md`](../nature-shared/core/discussion-argument-language.md).
- Main-text compression, figure/caption/SI allocation or revision accretion: load [`main-text-discipline.md`](../nature-shared/core/main-text-discipline.md).
- Exact journal limits and submission requirements: load the applicable file under [`nature-shared/journal-formats`](../nature-shared/journal-formats/), then verify the current official journal instructions.
- Initial submission packages and revision materials: use [`submission-and-revision.md`](references/submission-and-revision.md) under the workflow owner.

These are conditional references, not a second workflow and not official journal policy unless the linked source is an official current journal page. `nature-reviewer` remains a separate reviewer-side assessment skill.

## Full-manuscript bootstrap gate (H0)

Classify a request as **full-manuscript work** when it asks to write, rewrite, assemble or substantially restructure the whole paper. Run H0 before routing to a section owner or drafting complete prose. Record one status for every item as **PASS**, **BLOCKED** or **N/A with an evidence-based reason**:

1. Article type, target journal or publisher, language, source format, output format, template/class, bibliography style and figure dimensions.
2. Authoritative evidence inventory covering data, analyses, procedures, source manuscripts, existing figures, tables and Supplementary Information.
3. A framework-record scaffold containing the question, evidence boundary, open decisions, term-table scaffold and known dependencies.
4. A claim–source ledger scaffold for background, motivating drawbacks, method-dependent claims, novelty statements and relevant interpretation.
5. A visual and SI allocation scaffold showing which claims may require main displays, supplementary displays or an evidence-based N/A decision.
6. An output/package plan covering the expected main text, SI, references, figures, source files and compiled outputs.

A mandatory BLOCKED item prevents complete-prose drafting for that dependency. Produce only a dependency diagnosis, framework scaffold or explicitly provisional artifact until it is resolved. H1–H4 must then complete the framework record, term table, claim–evidence map and Results architecture before H5–H7 figure-linked Results production begins. A complete manuscript requires every applicable H0–H12 gate, with no silent omission. The interaction mode changes review granularity and never waives this gate.

## Decide the next step

For a new whole-paper task, a resume request, a change spanning sections or uncertainty about the next action, read [workflow-state.md](references/workflow-state.md). Reconstruct the current state from the conversation, existing decision record and actual artifacts. New or full-paper work starts at H0, then proceeds through the applicable dependency order. Preparation may be parallel when prerequisites allow, but every applicable checkpoint is required before H12 and no checkpoint may be silently skipped.

Track progress, author decisions and verification separately against the relevant artifact version. Update the existing record after a specialist returns or the author gives feedback. Preserve unaffected accepted work. Briefly state the next step, its owner and why it is ready or blocked, then carry out authorized work. A status-only question does not authorize expanding the task; a bounded section request goes directly to its owner without a whole-paper reassessment.

## Select the owner

| Requested work | Skill |
|---|---|
| Scientific question, contribution, drawback map, storyline and Results architecture | [manuscript-storyline](../manuscript-storyline/SKILL.md) |
| Title and Abstract | [manuscript-abstract](../manuscript-abstract/SKILL.md) |
| Introduction | [manuscript-introduction](../manuscript-introduction/SKILL.md) |
| Results subsections and conditional evidence reporting | [manuscript-results](../manuscript-results/SKILL.md) |
| Discussion, limitations and scientific ending | [manuscript-discussion](../manuscript-discussion/SKILL.md) |
| Methods, procedures and reproducibility description | [manuscript-methods](../manuscript-methods/SKILL.md) |
| Supplementary Information and its main-text connections | [manuscript-supplementary](../manuscript-supplementary/SKILL.md) |
| Figures, tables, panels, captions and Python plotting with figures4papers | [manuscript-figures](../manuscript-figures/SKILL.md) |
| Generic language-only polishing or translation of a bounded excerpt | [manuscript-polishing](../manuscript-polishing/SKILL.md) |
| Requested audit, pre-revision diagnosis and integrated evidence/consistency verification | [manuscript-audit](../manuscript-audit/SKILL.md) |

A section-specific request goes directly to that section's skill, including bounded local edits. Generic language polishing uses the polishing skill; it consults section rules only when that context matters. Selected Nature guidance is integrated into these owners; our contract, section requirements and accepted decisions govern conflicts. Use [integration notes](references/nature-integration.md) for provenance and maintenance boundaries. The separate `nature-reviewer` skill remains assessment-only and does not own manuscript authoring or polishing.

For any new or full-manuscript task, load [literature.md](references/literature.md) before H2 or H8 and maintain its claim–source ledger through H12. For bounded work, load it when substantive literature search, citation verification or reference export is in scope. Retain the current section owner, or use manuscript-audit for a reference audit. For requested initial-submission materials or reviewer correspondence, load [submission-and-revision.md](references/submission-and-revision.md). Neither route creates a new mode, authorizes external submission, nor starts unrelated research work.

## Coordinate the manuscript

For a new/full manuscript or revision across sections, read [workflow.md](references/workflow.md) for H0–H12 and revision routing. Inspect actual evidence before proposing the story. Run H0, then complete the H1–H4 framework record and term table, then the visual H5–H6 gates before treating Results prose as complete. Route bounded work to the relevant owner only after its prerequisites are present. Before full or substantive whole-manuscript revision, use manuscript-audit to diagnose structure, all sections and paragraph logic; then send bounded work to the relevant owner. Audit-only stays an audit.

Hand off the accepted question/contribution, sources and evidence limits, terminology, target/format, confirmed mode, protected material, approved decisions and current scope. Reuse the existing record rather than creating one per skill. Resolve a change's effects across sections, figures, captions, tables and SI; revisit accepted decisions only when materially affected. A brief edit can retain this context in the conversation.

For a complete research article, use this **production order** unless the article type provides a documented dependency exception: H0 intake → H1–H4 framework and Results architecture → H5 visual storyboard → H6 real-data figure prototypes → H7 Results and figure iteration → H8 Introduction → H9M Methods → H9S Supplementary Information → H10 Discussion → H11 final Abstract and title → H12 integrated package. The publication order may remain Abstract → Introduction → Results → Discussion → Methods → Supplementary Information. A provisional Abstract or Methods inventory may be prepared earlier only when explicitly labelled provisional. Final Introduction, Methods, Supplementary Information, Discussion and Abstract prose must use the stabilized Results and figure set. H9S is an independent gate and cannot be absorbed into Methods or silently omitted.

For post-review work, preserve original reports and map each comment to evidence, action, completion status, location and response under [submission-and-revision.md](references/submission-and-revision.md). Route substantive changes to the affected skills and follow the confirmed mode. A reviewer request alone does not authorize new experiments.

## Assemble and deliver

Lock the target journal or publisher template, source format, class/style, bibliography system, figure dimensions and output requirements at H0. If the target is unknown, mark the package **provisional** and do not describe generic output as journal-formatted. Retain the selected template and all figure/bibliography dependencies.

Assemble main text, SI, displays, legends, references and supporting material. Compile the actual main and supplementary sources, resolve every citation and bibliography record, and inspect equations, floats, tables, figures, captions, numbering, page fit and final-size artwork. Run the multi-pass manuscript audit in [audit.md](../manuscript-audit/references/audit.md#multi-pass-manuscript-audit) and report scientific support, terminology/defensive-language status, numerical reproduction, visual layers, compilation, layout, package completeness and venue compliance separately. A package is complete only when all applicable gates pass or carry an evidence-based N/A status.
Open the actual delivery package and check the editable main text, SI, compiled PDFs and submission letter together. Confirm that every main-text callout and hyperlink reaches the intended item, that SI figures and tables are visible under their printed numbers, and that each display shows the quantities described in the text. When files are consolidated or replaced, update the package manifest, links and any promises about attached data or code in the letter before removing superseded attachments. Verify the current journal's rules for separate data files and preserve internal reproducibility material at its authorized location.
