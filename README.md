# ZeroPlot

> **Plot anything. From zero.**

ZeroPlot is an agent skill for turning intent, data, or reference material into
editable visual artifacts.

## Scope

ZeroPlot starts with scientific figures, then expands across the visual stack:

```text
Charts → Diagrams → Figures → Posters → Slides
```

Inputs may include natural-language intent, datasets, source code, rough
sketches, screenshots, papers, netlists, structured specs, or existing visuals.

Outputs should remain editable whenever possible:

- SVG, draw.io, Mermaid, TikZ, matplotlib source, or structured JSON;
- PPTX or other structured slide formats;
- PDF and PNG exports for delivery;
- flat raster only when no editable route exists.

## Why ZeroPlot

Most visual work starts with format friction: choose a tool, translate intent
into its primitives, then rebuild the result whenever requirements change.
ZeroPlot makes intent the starting point and editability the contract.

`plot` means composing visual elements—not only statistical plotting.

## Skill

The installable skill lives at [`skills/zeroplot`](skills/zeroplot).

Initial domain packs:

- integrated circuits;
- computer science systems and pipelines.

Scientific figures are the first proving ground, not the product boundary.

## Install

### Codex

```bash
npx skills add blackblue-labs/zeroplot -g -a codex -y
```

### Manual

Copy `skills/zeroplot` into your agent's skill directory.

## Roadmap

- Strengthen chart, diagram, and schematic generation.
- Add editable poster and slide workflows.
- Build domain-aware visual rubrics and benchmark cases.
- Connect generation, reconstruction, editing, and export.

## License

MIT.
