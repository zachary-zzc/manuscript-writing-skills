# Related skill repositories

This repository keeps its core manuscript workflow self-contained. Related skill collections can be checked out beside it when you need to inspect upstream source material or work across repositories.

## Registry

The machine-readable registry is [`related-skills.yaml`](../related-skills.yaml). It records the repository URL, an optional checkout path, the relationship to this package, and the reference used when the local guidance was adapted.

| Repository | Relationship | Local integration |
| --- | --- | --- |
| [`Yuan1z0825/nature-skills`](https://github.com/Yuan1z0825/nature-skills) | Source reference for selected Nature guidance | [`nature-integration.md`](../skills/manuscript-workflow/references/nature-integration.md) |
| [`ChenLiu-1996/figures4papers`](https://github.com/ChenLiu-1996/figures4papers) | Source reference for figure-making patterns | [`manuscript-figures/references/figures4papers.md`](../skills/manuscript-figures/references/figures4papers.md) |
| [`Sleepy-Avacado/FigGenie`](https://github.com/Sleepy-Avacado/FigGenie) | Credited schematic-workflow reference | [`nature-integration.md`](../skills/manuscript-workflow/references/nature-integration.md) |

The package does not execute or import these repositories. Their references provide provenance and optional material for a focused comparison.

## Optional submodules

Add only the source repository you need:

```bash
git submodule add https://github.com/Yuan1z0825/nature-skills.git external/nature-skills
git submodule add https://github.com/ChenLiu-1996/figures4papers.git external/figures4papers
git submodule add https://github.com/Sleepy-Avacado/FigGenie.git external/FigGenie
git submodule update --init --recursive
```

The checkout paths match `related-skills.yaml`. Keep external repositories separate from `skills/` so the canonical package keeps one owner per behavior and upstream licenses remain visible at their original repository boundaries.

## Adding another related repository

1. Add one entry to `related-skills.yaml` with a stable URL, checkout path, role, and reference or commit.
2. Add a row to the table above with the local integration point.
3. Use `git submodule add` only when the repository is independently maintained and you need a local checkout. A link in the registry is enough for a reference that should remain remote.
4. Record the relevant license and attribution in the consuming skill's provenance note.
5. Re-run the link and package checks described in the root README.
