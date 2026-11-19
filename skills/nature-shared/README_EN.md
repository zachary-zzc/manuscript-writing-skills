# `nature-shared/` - shared support package for the canonical manuscript-* suite and nature-reviewer

This is an installable support package, not a standalone user workflow. It keeps the shared definitions and references used by the canonical manuscript-* suite and nature-reviewer in one place so those sources stay consistent and update together. A complete `npx skills` installation discovers and manages it alongside the user-facing skills.

Sibling skills reference these files through relative paths such as:

```yaml
always_load:
  - ../nature-shared/core/reader-workflow.md
```

## Contents

| File | Consumers |
|---|---|
| `core/reader-workflow.md` | `manuscript-polishing`, `manuscript-workflow` |
| `core/paper-type-taxonomy.md` | `manuscript-polishing`, `manuscript-workflow` |
| `core/ethics.md` | `manuscript-polishing`, `manuscript-workflow` |
| `core/research-compliance.md` | `manuscript-workflow` and skills needing Nature Portfolio specialist compliance checks |
| `core/terminology-ledger.md` | `manuscript-polishing`, `manuscript-workflow`, `nature-reader`, `nature-paper2ppt` |
| `core/consistency-sweep.md` | `manuscript-polishing`, `nature-reviewer` and other review consumers |
| `core/main-text-discipline.md` | `manuscript-workflow`, `manuscript-polishing` and revision consumers |
| `core/nature-results-discussion.md` | Nature / Nature Portfolio Results claim escalation and Discussion synthesis for `manuscript-workflow` and `manuscript-polishing`, distilled from published NMI and flagship Nature papers (not official policy) |
| `core/discussion-argument-language.md` | Journal-general Discussion functions, reverse-funnel control, evidence-calibrated modality, claim boundaries, and future-work auditing for `manuscript-workflow` and `manuscript-polishing` (writing guidance, not journal policy) |
| `core/nature-introduction.md` | Nature / Nature Portfolio problem funnels, exact gaps, and Introduction–Results alignment for `manuscript-workflow` and `manuscript-polishing`, initially distilled from NMI papers (not official policy) |
| `core/nature-abstract.md` | Nature / Nature Portfolio discovery-centred abstract evidence chains, claim hierarchy, and numeric selection for `manuscript-workflow` and `manuscript-polishing`, initially distilled from NMI papers (not official policy) |
| `journal-formats/nat-comms.md` | `manuscript-polishing`, `manuscript-workflow` |
| `journal-formats/nature.md` | `manuscript-workflow` and skills needing exact flagship `Nature Article` submission rules |
| `journal-formats/nature-machine-intelligence.md` | Writing, polishing, figure, data, and statistics workflows for NMI submissions |

`scripts/check_consistency.py` provides a mechanical first pass for terminology variants, equal values reported at different precision, and equivalent lengths expressed in different units. Its output is a set of warnings for contextual review, not automatic edits.

## When to Put Files Here

Only place a file here when two or more skills need to reuse the same content. If the content serves only one skill, keep it in that skill's own `static/` or `references/` directory.

## When to Keep Content Local

The shared layer should hold definitions and references only, such as paper-type classifications, reader workflows, ethics rules, or terminology ledgers. Skill-specific diagnosis, drafting, modification, and output logic should remain in each skill's own files.

## Relationship With Other Skills

`nature-shared/` is not a standalone workflow. It is a shared dependency package that the canonical manuscript-* skills and nature-reviewer read on demand.
