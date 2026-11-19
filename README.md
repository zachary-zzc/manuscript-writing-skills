# Manuscript Skills

A coordinated skill package for planning, writing, polishing, auditing, and assembling scientific manuscripts with evidence boundaries and reproducible review checkpoints.

The package is designed for Codex-style skill loading. It contains the complete `manuscript-*` suite plus the shared `nature-shared` reference package that the suite loads on demand.

## What is included

| Skill | Responsibility |
| --- | --- |
| [`manuscript-workflow`](skills/manuscript-workflow/SKILL.md) | Coordinates whole-paper work, revisions, submission packages, and hand-offs |
| [`manuscript-storyline`](skills/manuscript-storyline/SKILL.md) | Builds the evidence-backed question, contribution, drawback map, and Results architecture |
| [`manuscript-abstract`](skills/manuscript-abstract/SKILL.md) | Drafts and verifies titles and Abstracts |
| [`manuscript-introduction`](skills/manuscript-introduction/SKILL.md) | Develops the problem, knowledge gap, and contribution |
| [`manuscript-results`](skills/manuscript-results/SKILL.md) | Reports supported findings with claim–evidence–display alignment |
| [`manuscript-discussion`](skills/manuscript-discussion/SKILL.md) | Interprets findings, limitations, and supported implications |
| [`manuscript-methods`](skills/manuscript-methods/SKILL.md) | Describes actual procedures, inputs, assumptions, and reproducible analyses |
| [`manuscript-supplementary`](skills/manuscript-supplementary/SKILL.md) | Organises supporting information and its links to the main text |
| [`manuscript-figures`](skills/manuscript-figures/SKILL.md) | Plans and verifies figures, tables, captions, and layout |
| [`manuscript-polishing`](skills/manuscript-polishing/SKILL.md) | Performs bounded language polishing and translation while preserving meaning |
| [`manuscript-audit`](skills/manuscript-audit/SKILL.md) | Audits structure, evidence, numbers, statistics, terminology, displays, and package completeness |
| [`nature-shared`](skills/nature-shared/SKILL.md) | Supplies shared Nature-related references to dependent skills on demand |
| [`nature-reviewer`](skills/nature-reviewer/SKILL.md) | Runs reviewer-side assessment with independent evidence and severity checks |

`nature-shared` is a dependency package. It is not a standalone writing workflow.

The reviewer skill is a separate assessment workflow. It shares the package's references but does not author or polish manuscript prose.

## Related skill repositories

Related Nature and visualization repositories are tracked in [`related-skills.yaml`](related-skills.yaml). Read [`docs/related-skills.md`](docs/related-skills.md) for provenance, optional submodule commands, and the rule for adding another independently maintained skill repository. The core package does not require these external checkouts.

## Design principles

- **One owner per behavior.** Section skills own section work, `manuscript-polishing` owns language editing, `manuscript-figures` owns visual verification, `manuscript-audit` owns integrated checks, and `manuscript-workflow` routes cross-section work.
- **Evidence before wording.** Claims stay attached to the actual study object, comparison, population, condition, version, and display that support them.
- **Bounded scope.** Local edits remain local unless the evidence or requested change requires wider reconciliation.
- **Explicit uncertainty.** Missing author facts, unresolved provenance, and unassessed checks remain visible instead of being inferred or silently repaired.
- **On-demand references.** Shared and journal-specific guidance is loaded only when the task requires it.

## Installation

Copy the `skills/` directory into the skill directory used by your agent:

```bash
cp -R skills/* ~/.codex/skills/
```

The package preserves the relative paths used by the skill files. Keep all sibling directories together so links such as `manuscript-workflow → nature-shared` continue to resolve.

If your environment uses another skill root, copy the same directory contents there. The package does not require a Python runtime for ordinary manuscript drafting. The optional consistency checker requires Python 3.10 or newer.

## Typical entry points

Use the workflow manager when the task spans sections or the next manuscript step is unclear:

```text
Use $manuscript-workflow to assess the current manuscript state and continue with the next evidence-backed step.
```

Use a section skill for bounded work:

```text
Use $manuscript-results to revise this Results subsection while preserving the accepted evidence and claim strength.
```

Use the audit skill for explicit pre-revision or integrated verification:

```text
Use $manuscript-audit to audit the manuscript at the requested scope and separate confirmed findings from evidence gaps.
```

## Consistency checker

The shared package includes a mechanical first-pass checker for terminology variants, numeric precision variants, and equivalent length units:

```bash
python skills/nature-shared/scripts/check_consistency.py path/to/manuscript.md
```

The checker reports risks for human review. It does not rewrite manuscript text. Run its regression tests with:

```bash
python -m unittest discover -s skills/nature-shared/tests -v
```

The reviewer contract tests use pytest-style functions:

```bash
pytest -q skills/nature-reviewer/tests/test_reviewer_instruction_contracts.py
```

## Package layout

```text
skills/
├── manuscript-abstract/
├── manuscript-audit/
├── manuscript-discussion/
├── manuscript-figures/
├── manuscript-introduction/
├── manuscript-methods/
├── manuscript-polishing/
├── manuscript-results/
├── manuscript-storyline/
├── manuscript-supplementary/
├── manuscript-workflow/
├── nature-reviewer/
└── nature-shared/
```

Each skill keeps its own `SKILL.md`, optional agent metadata, and scoped references. The workflow and section files link to sibling packages rather than duplicating shared guidance.

## Provenance and licensing

The `nature-shared` package includes its upstream attribution and the included Apache License 2.0 notice in [`nature-integration.md`](skills/manuscript-workflow/references/nature-integration.md) and [`NATURE-APACHE-2.0.txt`](skills/manuscript-workflow/licenses/NATURE-APACHE-2.0.txt). The figures guidance records the separately attributed `figures4papers` material and its CC BY-NC 4.0 terms where applicable.

The repository does not add a blanket license for the full manuscript suite. Review the per-file provenance and license notes before redistributing or adapting individual materials.

## Status

This repository is a public snapshot of the coordinated skill package. Journal limits and submission requirements remain subject to the current official journal instructions, which should be verified at the time of use.
