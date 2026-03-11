# Key Components of Algorithm Auditing — 2

## Ways to audit / levels of access:
- More granular than "white-box" and "black-box" — based on knowledge/access to the components behind the learning process

| Level | Access | What you can assess |
|-------|--------|-------------------|
| Level 1 | Process access | Checklists, guidelines |
| Level 2 | Model access | Feature relevance, adversarial attacks, adversarial fairness, statistical disclosure |
| Level 3 | Input access f(x) | Surrogate explanations, synthetic data, bias in outcome, property inference |
| Level 4 | Outcome access f(x), y | Accuracy of explanations, concept drift, bias in opportunity, inversion attacks |
| Level 5 | Parameter control f_θ(x), y | Stability of explanations/bias metrics, stress-testing, functionality stealing |
| Level 6 | Learning goal L(f_θ(x), y) | Model complexity, model selection, trade-off of bias and loss metric, model extraction |
| Level 7 | White-box | Documents and specific explanations, full model selection and validation/development, model security evaluation |
