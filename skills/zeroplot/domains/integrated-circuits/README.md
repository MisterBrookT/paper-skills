# Integrated Circuits

Seed domain for ZeroPlot.

## Target User

Circuit researchers who already have a design and need a paper-ready,
editable schematic illustration.

## Figure Families

- transistor-level analog schematic illustration;
- switched-capacitor schematic;
- differential circuit schematic;
- mixed signal architecture block diagram;
- simulation/timing plot with circuit-specific annotations.

## Inputs

- SPICE/netlist;
- rough EDA schematic screenshot;
- paper text or figure caption;
- hand sketch;
- component and connection table;
- visual reference from a paper.

## Output

Preferred:

- `.drawio`;
- SVG;
- PDF/PNG export for manuscript insertion;
- drawing spec JSON for reproducibility.

## Hard-Fail Criteria

- component symbols are not circuit symbols;
- MOS, capacitors, switches, supplies, grounds, or differential ports are wrong;
- connectivity changes the circuit meaning;
- signal flow is ambiguous;
- symmetry is broken where the circuit is symmetric;
- labels, phases, sizes, or common-mode markers are missing;
- line crossings make the schematic unreadable.

## Benchmark Loop

```text
input materials
  -> baseline draw.io/SVG
  -> expert marks why it does not look like an IC paper figure
  -> rubric.yaml
  -> skill rule update
  -> held-out case
```
