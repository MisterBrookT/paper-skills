# `plot`

Discipline-aware scientific figures for research papers.

## Why This Exists

Academic figures are not one universal genre. A circuit schematic, a biology
pathway, an AI system diagram, and a finance risk figure use different inputs,
symbols, layout conventions, and expert criteria.

`plot` captures those differences as skills, rubrics, and benchmark cases.

## First Milestone

Integrated-circuit seed bench:

```text
query -> baseline -> expert failure notes -> rubric -> skill v0 -> held-out eval
```

## Domain Cases

| Domain | Path | Status | Figure Families |
| --- | --- | --- | --- |
| Integrated circuits | `domains/integrated-circuits/` | seed | analog schematic illustrations, switched-capacitor diagrams, architecture blocks |
| Computer science | `domains/computer-science/` | seed | system diagrams, model architecture, pipeline/dataflow, evaluation setup |

Planned later:

- biology mechanisms/pathways;
- finance figures;
- materials mechanisms.

## Shared Loop

Every domain should define:

- inputs;
- figure families;
- hard-fail criteria;
- visual grammar;
- editable output format;
- benchmark cases.
