# Challenges of Explainability

## No agreed definition
- There is no standard definition or measurement of "explainability" or "transparency"
- What counts as a good explanation is context-dependent

## Explanations require domain knowledge
- A saliency map highlighting regions of an **X-ray** is meaningless to someone without medical training
- Explanations must be designed for their **audience**, not just for technical correctness

## Explainers disagree with each other
- Swamy et al. (2022) compared LIME, KernelSHAP, PermSHAP, CEM, and DiCE on the same data
- PCA of explainer outputs clustered **by method, not by dataset** — each method measures something different
- No single explainer gives the "true" explanation

## Implication for practice
- Use **multiple explanation methods** and compare critically
- Treat explanations as **hypotheses**, not ground truth
