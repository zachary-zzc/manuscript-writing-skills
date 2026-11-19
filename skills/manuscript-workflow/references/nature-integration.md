# Nature guidance: sources and integration boundaries

This is a maintenance reference, not an additional drafting workflow. Selected guidance was adapted and rewritten on 2026-10-28 from [Yuan1z0825/nature-skills](https://github.com/Yuan1z0825/nature-skills/tree/4a04b953c13c57adc51e202ce296597f00d29d67), commit `4a04b953c13c57adc51e202ce296597f00d29d67`. The repository is an author-maintained skill collection, not official Nature Portfolio policy.

The existing manuscript suite remains the standard where guidance conflicts. Its confirmed Easy/Normal/Expert mode, accepted decisions, section structure and length requirements, evidence boundaries and delivery defaults remain in force. Current explicit user instructions and applicable higher-priority instructions govern as before; surface a conflict with verified venue requirements rather than silently changing an author default.

## Canonical active architecture

The 11 `manuscript-*` skills are the canonical authoring, editing, figures and audit suite. Nature-specific writing and polishing are journal modes within those owners, supported by the references in `nature-shared`; they are not separate authoring workflows. The former `nature-writing` and `nature-polishing` routers were retired on 2026-11-06 and preserved in the local skills archive for rollback or selective migration. `nature-reviewer` remains separate because it evaluates from the reviewer side rather than drafting or polishing author prose.

The active rule is one owner per behavior: section owners write sections, `manuscript-polishing` owns language editing, `manuscript-figures` owns visual design and verification, `manuscript-audit` owns integrated QA, and `manuscript-workflow` routes whole-paper and submission work.

### Active routing map

| Request | Canonical owner | Nature guidance to load when relevant |
|---|---|---|
| Title or Abstract | `manuscript-abstract` | `nature-shared/core/nature-abstract.md` |
| Storyline or Introduction | `manuscript-storyline` or `manuscript-introduction` | `nature-shared/core/nature-introduction.md` |
| Results | `manuscript-results` | `nature-shared/core/nature-results-discussion.md` and `main-text-discipline.md` |
| Discussion or conclusion | `manuscript-discussion` | `nature-results-discussion.md` and `discussion-argument-language.md` |
| Methods or Supplementary Information | `manuscript-methods` or `manuscript-supplementary` | `main-text-discipline.md` when placement or compression is in scope, plus current journal requirements |
| Figures, captions or layout | `manuscript-figures` | `visual-form-selection.md`, `nature-shared/journal-formats/*` and `latex-layout.md` as applicable |
| Generic polishing or translation | `manuscript-polishing` | The relevant Nature corpus or journal-format reference only when the target requires it |
| Whole-manuscript, submission or revision package | `manuscript-workflow` | `nature-shared` references plus `submission-and-revision.md` and current official instructions |
| Pre-submission reviewer simulation | `nature-reviewer` | Reviewer references only; do not turn review into authoring |

## Source mapping

The links below identify the exact inspected revision. The integrated references contain selected adaptations, not complete copies or a promise to track upstream automatically.

| Local owner / reference | Upstream material and selected contribution |
|---|---|
| Introduction | [nature-introduction](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-shared/core/nature-introduction.md): motivation and answer coverage. |
| Storyline / Results / SI / paragraph review | [nature-results-discussion](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-shared/core/nature-results-discussion.md), [main-text-discipline](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-shared/core/main-text-discipline.md): distinct inferential roles, placement and repetition checks. |
| Discussion / shared writing style | [discussion-argument-language](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-shared/core/discussion-argument-language.md): literature relationships, rival explanations and modal meanings. That source credits an author-supplied discussion-writing article and *Science Research Writing for Non-native Speakers of English*; no book text is reproduced here. |
| [Literature](literature.md) | [Citation workflow](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-citation/static/core/workflow.md), [claim search](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-citation/references/search-strategy.md), [reference verification](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-ref-verifier/SKILL.md), [deduplication](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-academic-search/references/dedup-engine.md), [database search](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-academic-search/references/search-strategy.md): support grading, search records and field-level metadata checks. |
| Audit statistical reporting | [Failure modes](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-statistics/references/common-failure-modes.md), [reporting](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-statistics/references/statistical-reporting.md): interaction interpretation, report fields, assumptions and exclusion history. |
| Audit data availability, shared with Methods and SI | [Data workflow](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-data/static/core/workflow.md), [repositories](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-data/references/repository-and-identifiers.md), [metadata](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-data/references/fair-metadata-checklist.md): dataset/access/citation mapping and scoped reuse checks. |
| Figures | [QA contract](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-figure/references/qa-contract.md), [schematic workflow](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-figure/references/vector-schematic-workflow.md), [schematic semantics](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-figure/references/vector-schematic-style-rules.md): final-render geometry, current-export collisions, edge evidence and image history. |
| [Submission and revision](submission-and-revision.md) | [Initial package](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-writing/references/submission-package.md), [response workflow](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-response/static/core/workflow.md), [package consistency](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-response/references/package-consistency-audit.md): factual submission materials and comment/change/response reconciliation within the existing manager. |

## Deliberate adaptations

The audit owner's [domain-evidence.md](../../manuscript-audit/references/domain-evidence.md) also selectively adapts [domain-specific-review-gates](https://github.com/Yuan1z0825/nature-skills/blob/4a04b953c13c57adc51e202ce296597f00d29d67/skills/nature-reviewer/references/domain-specific-review-gates.md): measurement proxies, independent validation, operating range and scale of inference. It is a conditional example reference, not a new reviewer or universal checklist.

- Keep eleven skill entries and one canonical owner per rule. Abstract and polishing inherit shared improvements without duplicate rule sets. Load specialised checks only for the requested work and actual study objects.
- Keep inference/placement checks in existing records; do not require extra ledgers or shorten complete sections below personal requirements. Preserve conclusion-changing negative, subgroup and robustness evidence in main text.
- Select literature by scientific relevance. Do not import journal-prestige filters, arbitrary metadata-error thresholds or the claim that a Crossref lookup failure proves a DOI invalid.
- Do not import a fixed reviewer count, automatic new analyses, universal figure geometry tolerances, backend-selection questions, forced response-file separation or prescribed revision colours. No new ordinary approval checkpoints are introduced.
- Upstream scripts, APIs, templates and dependencies are not bundled or executed. The figure rules describe verification protocols; tool availability and actual execution determine which checks can be reported as performed. Existing figures4papers integration is unchanged.
- Reading/translation products, slide/Word converters, patents, research proposals, experiment logs, downloads and scheduled literature monitoring remain outside this integration. Their relevant outputs may supply evidence when requested.

## Licence and attribution

The inspected upstream material is covered by the repository's [Apache License 2.0](../licenses/NATURE-APACHE-2.0.txt), included unchanged. No applicable NOTICE file was present in the pinned tree. Its schematic workflow also credits the independent MIT-licensed [FigGenie](https://github.com/Sleepy-Avacado/FigGenie) for its workflow structure; none of that project's code, figures, parts or fonts is bundled here. The selected additions have been rewritten and scoped for this suite; source notes identify adapted files. This attribution does not relicense pre-existing personal guidance or the separately attributed figures4papers material. Future upstream updates require a fresh comparison against the local contract, not wholesale replacement.
