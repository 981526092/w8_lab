# Mechanistic Interpretability: Summary

## The toolkit:

| Method | Question it answers | Approach |
|--------|-------------------|----------|
| **Linear Probes** | What information is encoded at each layer? | Train linear classifier on frozen activations |
| **Superposition** | Why are individual neurons hard to interpret? | Features outnumber neurons; stored as overlapping directions |
| **Sparse Autoencoders** | What are the true features? | Learn a sparse, overcomplete dictionary of monosemantic features |
| **Activation Patching** | Which components cause a specific behavior? | Causal intervention — swap activations between runs |

## From post-hoc to mechanistic:
- **SHAP/LIME** → "Which input features matter?" (input-level)
- **Mech. Interp.** → "What computations does the model perform internally?" (model-level)

## Open challenges:
- Scaling SAEs to very large models (billions of features?)
- Ensuring discovered features are **faithfully** used by the model (not just correlated)
- Connecting individual features into full **circuits** that explain complex behaviors
