# Paper Skills

**Journal-ready AI skills for every research discipline.**

Paper Skills is an open skill library for research-paper workflows. It curates
strong public academic skills and adds first-party work where research papers
still need domain taste: scientific figures.

## What This Is

Most academic AI skills help with writing, literature review, citation checks,
or reviewer response. Those are important, but many good open projects already
cover them.

Paper Skills starts from a sharper thesis:

> Every discipline has its own research-paper language. That language includes
> prose, evidence, citations, review expectations, and figures.

The first original module is `plot`: discipline-aware scientific figures for
papers.

## Flagship: `plot`

`skills/plot` turns domain materials into editable, paper-ready figures.

```text
domain input
  -> baseline figure
  -> expert failure notes
  -> rubric
  -> skill evolution
  -> adaptive benchmark
```

Initial cases:

- **Integrated circuits**: transistor-level analog schematic illustrations from
  netlists, EDA screenshots, paper text, sketches, and component tables.
- **Computer science**: system diagrams, model architecture figures, pipelines,
  dataflow diagrams, and benchmark/evaluation setup figures.

The goal is not generic prettiness. The goal is for domain experts to say:
this looks like a figure from our field.

## Curated Skills

Writing, citation, review, and venue-specific packs begin as curated entry
points. Paper Skills should integrate or reference strong public skill projects
instead of copying them blindly.

```text
skills/
  plot/          first-party discipline-aware figure workflow
  writing/       curated writing and polishing entry points
  citation/      curated citation and reference checks
  review/        reviewer response and manuscript QA
  venue-packs/   journal- and discipline-specific packs
```

## Repository Layout

```text
skills/
  plot/
    domains/
      integrated-circuits/
      computer-science/
  writing/
  citation/
  review/
  venue-packs/
docs/
  academic-skill-pack-survey.md
integrations/
  catalog.md
registry.yaml
```

## Status

Draft scaffold. APIs, install flow, and copied integrations are not stable yet.

