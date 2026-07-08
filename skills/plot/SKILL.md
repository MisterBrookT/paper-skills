---
name: plot
description: >-
  Use for discipline-aware scientific figure generation, figure redesign,
  paper-ready schematic illustrations, domain-specific visual grammar,
  expert rubric extraction, adaptive figure benchmarks, and editable figure
  outputs for research papers.
---

# Plot Skill

`plot` is the original flagship skill in Paper Skills. It focuses on
paper-ready scientific figures across disciplines, not generic chart styling.

## Core Scope

Use this skill when the user needs:

- a discipline-specific research figure;
- an editable scientific schematic or diagram;
- a figure generated from domain materials such as netlists, paper text,
  pathway notes, system descriptions, time-series events, or rough sketches;
- an expert-review rubric for what makes a figure acceptable in a field;
- a benchmark case for domain-aware figure generation.

## Non-Goals

- Do not claim to replace professional EDA, CAD, statistical, or simulation
  tools.
- Do not optimize only for visual prettiness.
- Do not turn field-specific figures into generic PowerPoint-style diagrams.
- Do not invent scientific content not present in the user's materials.

## Workflow

1. Identify domain and figure family.
2. Collect source materials and constraints.
3. Convert inputs into an auditable drawing spec.
4. Produce a baseline figure in an editable format when possible.
5. Ask for or infer domain-specific failure criteria.
6. Distill failures into rubric items and skill rules.
7. Re-run generation with the updated rules.
8. Save benchmark artifacts when the task is part of evaluation.

## Domain Contract

Before generation, write a short contract:

- domain;
- figure family;
- source inputs;
- target output format;
- must-preserve entities and relationships;
- hard-fail criteria;
- stylistic conventions;
- evaluation plan.

## Output Preference

Prefer editable outputs over flat images:

1. `.drawio`, SVG, Mermaid, TikZ, matplotlib source, or structured JSON;
2. PDF/PNG export for manuscript insertion;
3. flat raster only when no editable route is available.

## First Domain: Circuit Figures

Initial seed domain:

```text
transistor-level analog schematic illustration
```

Goal: turn existing circuit materials into paper-ready schematic
illustrations. Inputs may include SPICE/netlist, rough EDA screenshots,
paper text, hand sketches, component tables, and visual references.

The target is not circuit design automation. The target is scientific figure
automation for readable, editable, publication-ready circuit illustrations.

