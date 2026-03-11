# Why Mechanistic Interpretability?

## Limitations of post-hoc methods (SHAP, LIME, etc.)
- They explain **what** features matter, but not **how** the model processes them internally
- Explanations can be unstable or misleading (e.g., LIME's local approximation may not reflect global behavior)
- No insight into the internal **representations** or **algorithms** learned by the model

## Mechanistic Interpretability aims to:
- Reverse-engineer the **internal computations** of neural networks
- Identify meaningful **features** and **circuits** within the model
- Understand **how** models arrive at their outputs, not just which inputs are important

## Key idea:
- Neural networks learn **representations** (features) in their activations
- These representations can be studied, extracted, and understood
