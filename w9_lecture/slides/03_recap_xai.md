# Recap: Explainability So Far

Last week we covered **post-hoc, model-agnostic** methods:
- **Permutation Feature Importance** — which features matter most?
- **SHAP** — Shapley values for fair credit assignment to features
- **LIME** — local surrogate models for individual predictions

These methods treat the model as a **black box** — they probe inputs and outputs.

**This week's question:** Can we open the black box and look *inside* neural networks?

> This is the domain of **Mechanistic Interpretability** — understanding the internal computations (representations and circuits) learned by neural networks.
