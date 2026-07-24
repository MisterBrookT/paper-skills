<div align="center">

# ZeroPlot

### Plot anything. From zero.

Turn intent, data, or references into editable visual artifacts.

[![Status](https://img.shields.io/badge/status-alpha-1677ff?style=flat-square)](https://github.com/blackblue-labs/zeroplot)
[![Agent Skill](https://img.shields.io/badge/Agent-Skill-05070d?style=flat-square)](skills/zeroplot)
[![License](https://img.shields.io/badge/license-MIT-05070d?style=flat-square)](LICENSE)
[![Black Blue Labs](https://img.shields.io/badge/Black_Blue-Labs-0b2a6f?style=flat-square)](https://github.com/blackblue-labs)

[中文](README.zh.md)

</div>

![ZeroPlot — one origin, many editable visual artifacts](assets/zeroplot-hero.webp)

## One visual system. Every format.

ZeroPlot is an Agent Skill for creating and redesigning structured visuals.
It starts from what you mean—not which drawing tool you know.

```text
Intent / Data / Reference
            ↓
        Visual Spec
            ↓
Chart · Diagram · Figure · Poster · Slide
            ↓
     Editable Source + Export
```

`plot` means composing visual elements, not only statistical plotting.

## What it creates

| Artifact | Typical inputs | Preferred outputs |
| --- | --- | --- |
| Charts | datasets, metrics, tables | matplotlib, SVG, PDF, PNG |
| Diagrams | system descriptions, code, rough sketches | draw.io, SVG, Mermaid |
| Technical figures | papers, netlists, screenshots, domain specs | TikZ, SVG, draw.io |
| Posters | narrative, figures, brand constraints | PPTX, SVG, PDF |
| Slides | outline, evidence, existing deck | PPTX, structured slide source |

Scientific figures are the first proving ground—not the product boundary.

## Core contract

ZeroPlot optimizes for four things:

1. **Intent first** — start from meaning and constraints.
2. **Structure preserved** — keep entities, relationships, and data auditable.
3. **Editable by default** — prefer source formats over flattened pixels.
4. **Domain aware** — visual grammar changes across fields and audiences.

## Install

### Codex

```bash
npx skills add blackblue-labs/zeroplot -g -a codex -y
```

### Manual

Copy [`skills/zeroplot`](skills/zeroplot) into your agent's skill directory.

## Try it

```text
Use ZeroPlot to turn this CSV into a publication-ready editable chart.

Reconstruct this screenshot as an editable draw.io system diagram.

Turn this technical report into a five-slide visual narrative.
```

## Initial domain packs

| Domain | Coverage | Status |
| --- | --- | --- |
| [Integrated circuits](skills/zeroplot/domains/integrated-circuits) | schematics, switched-capacitor diagrams, architecture blocks | seed |
| [Computer science](skills/zeroplot/domains/computer-science) | systems, models, pipelines, evaluation setups | seed |

## Roadmap

- Chart, diagram, and schematic generation
- Reference-image reconstruction into editable structure
- Poster and slide workflows
- Domain rubrics and held-out visual benchmarks
- Generation → editing → export loop

## License

MIT. Built by [Black Blue Labs](https://github.com/blackblue-labs).
