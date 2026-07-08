# Computer Science

Seed domain for `plot`.

## Target User

CS, AI, systems, and data researchers who need paper-ready architecture,
pipeline, system, or evaluation figures.

## Figure Families

- model architecture diagram;
- system overview;
- pipeline/dataflow figure;
- computation graph;
- training or inference workflow;
- evaluation setup;
- ablation or benchmark map when a normal chart is insufficient.

## Inputs

- paper method section;
- model/module list;
- dataflow description;
- code or config snippets;
- rough sketch;
- existing figure screenshot;
- experiment table or benchmark setup notes.

## Output

Preferred:

- SVG;
- `.drawio`;
- Mermaid for simple flow diagrams;
- TikZ when the paper source needs LaTeX-native output;
- PDF/PNG export for manuscript insertion.

## Hard-Fail Criteria

- module boundaries are unclear;
- arrows do not encode data/control flow correctly;
- training, inference, and evaluation paths are mixed;
- tensor/data shapes or key labels are missing when necessary;
- visual hierarchy hides the main contribution;
- figure looks like a generic business flowchart instead of a CS paper figure.

## Benchmark Loop

```text
paper text / rough diagram
  -> baseline system figure
  -> expert failure notes
  -> rubric.yaml
  -> skill rule update
  -> held-out case
```

