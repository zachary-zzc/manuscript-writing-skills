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

## Decide the next step

For a new whole-paper task, a resume request, a change spanning sections or uncertainty about the next action, read [workflow-state.md](references/workflow-state.md). Reconstruct the current state from the conversation, existing decision record and actual artifacts. Choose the next action from the requested scope, unmet dependencies, pending reviews and verification results; H1–H12 are checkpoints rather than a mandatory linear queue.

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

For substantive literature search, citation verification or reference export, load [literature.md](references/literature.md); retain the current section owner, or use manuscript-audit for a reference audit. For requested initial-submission materials or reviewer correspondence, load [submission-and-revision.md](references/submission-and-revision.md). Neither route creates a new mode, authorizes external submission, nor starts unrelated research work.

## Coordinate the manuscript

For a new/full manuscript or revision across sections, read [workflow.md](references/workflow.md) for H1–H12 and revision routing. Inspect actual evidence before proposing the story. Before full or substantive whole-manuscript revision, use manuscript-audit to diagnose structure, all sections and paragraph logic; then send bounded work to the relevant owner. Audit-only stays an audit.

Hand off the accepted question/contribution, sources and evidence limits, terminology, target/format, confirmed mode, protected material, approved decisions and current scope. Reuse the existing record rather than creating one per skill. Resolve a change's effects across sections, figures, captions, tables and SI; revisit accepted decisions only when materially affected. A brief edit can retain this context in the conversation.

For a complete research article, default to Abstract → Introduction → Results → Discussion → Methods → Supplementary Information unless the author or verified target format governs otherwise. Integrate conceptual motivation into the Introduction and formal derivations into Methods; do not add a separate pre-Results theory or concluding section by habit. Preserve other article types and local scope. Section-specific word/paragraph requirements belong to their respective skills and must be verified when applicable.

For post-review work, preserve original reports and map each comment to evidence, action, completion status, location and response under [submission-and-revision.md](references/submission-and-revision.md). Route substantive changes to the affected skills and follow the confirmed mode. A reviewer request alone does not authorize new experiments.

## Assemble and deliver

Default saved full-manuscript delivery to an editable LaTeX project and compiled PDF unless the author requests another format or an existing source format governs. Select an appropriate journal/publisher template from an authoritative source and retain its class, style, bibliography and figure dependencies. Identify it accurately without implying journal acceptance or compliance. A generic article class is not an official template.

Assemble main text, SI, displays, legends, references and supporting material. Compile the actual main and supplementary sources, resolve citations/references and inspect equations, floats, tables, figures and page fit. Use manuscript-audit for integrated verification and report its separate readiness states. The shared contract controls final review and feedback learning; no new mode selection is needed when a specialist hands work back.
