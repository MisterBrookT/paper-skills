# Paper Skills

Journal-ready AI skills for every research discipline.

Paper Skills is an open skill library for research-paper workflows. It starts
as a curated, agent-readable skill hub and leaves room for a future product
surface.

## Positioning

Paper Skills has two layers:

- Curated research skills: writing, citation, review response, literature
  workflows, and venue packs can integrate or reference the best public skill
  projects instead of rebuilding everything.
- Original plot work: `skills/plot` is the flagship module for
  discipline-aware scientific figures.

## Why plot first

Many writing and polishing workflows are already well-covered by public
academic skill packs. Scientific figures remain more domain-sensitive:
circuits, biology pathways, AI system diagrams, finance figures, and materials
mechanism diagrams each use different inputs, symbols, visual grammar, and
expert criteria.

`plot` is where Paper Skills should be original:

```text
domain input
  -> baseline generation
  -> expert failure notes
  -> rubric
  -> skill evolution
  -> adaptive benchmark
```

## Repository Layout

```text
skills/
  plot/          discipline-aware scientific figure workflow
  writing/       curated writing/polishing entry points
  citation/      curated citation and reference checks
  review/        reviewer response and manuscript QA
  venue-packs/   journal- and discipline-specific packs
docs/
  academic-skill-pack-survey.md
integrations/
  catalog.md
registry.yaml
```

## Status

Draft scaffold. Do not treat current skills as production-ready.

