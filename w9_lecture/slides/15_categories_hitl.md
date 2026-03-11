# Categories of HITL-ML

## Learning with Humans — Who is in control?

```
Active Learning (Model controls):
  ┌───────┐  "label this"  ┌────────┐
  │ Model │───────────────▶│ Human  │
  │       │◀───────────────│(oracle) │
  └───────┘   label back   └────────┘

Interactive ML (Shared control):
  ┌───────┐  feedback ⇄    ┌────────┐
  │ Model │◀══════════════▶│ Human  │
  │       │  corrections   │(expert) │
  └───────┘                └────────┘

Machine Teaching (Human controls):
  ┌────────┐  curriculum   ┌────────┐
  │ Human  │──────────────▶│ Model  │
  │(teacher)│ designed data │(student)│
  └────────┘               └────────┘
```

| Category | Control | Description |
|----------|---------|-------------|
| **Active Learning (AL)** | Model | Model selects data, human labels it |
| **Interactive Machine Learning (IML)** | Shared | Human and model collaborate iteratively |
| **Machine Teaching (MT)** | Human | Human designs curriculum for the model |

## Beyond Learning:
- **Curriculum Learning (CL):** Organize dataset by increasing complexity
- **Explainable AI (XAI):** Explaining model decisions to humans
- **Usable AI / Useful AI:** Making AI accessible and satisfying user needs

> Taxonomy from Mosqueira-Rey et al. (2023)
