# Sparse Autoencoders (SAEs)

## The Solution to Superposition
- If features are stored in superposition, we need a way to **disentangle** them
- Sparse Autoencoders learn a **dictionary of interpretable features** from model activations

## Architecture:

```
┌─────────────┐     ┌──────────────────┐     ┌─────────────┐
│ Activation  │     │ Sparse Features  │     │Reconstructed│
│  (d=512)    │────▶│  (n=16384)       │────▶│  (d=512)    │
└─────────────┘     └──────────────────┘     └─────────────┘
                    │ ■ ■ □ □ □ □ □ □  │
     Encoder        │ □ □ □ ■ □ □ □ □  │      Decoder
                    │ □ □ □ □ □ □ ■ □  │
                    │  ~50 of 16K active│
                    │  + L1 sparsity    │
```

## Training objective:
- **Reconstruction loss:** the decoded output should match the original activation
- **Sparsity penalty (L1):** encourage most features to be zero → each feature should capture a distinct, interpretable concept

## Result:
- Each learned feature (dictionary element) often corresponds to a **monosemantic concept**
  - E.g., "code in Python", "the Golden Gate Bridge", "expressions of uncertainty", "legal language"
- Far more interpretable than looking at individual neurons

> Reference: Cunningham et al. (2023), "Sparse Autoencoders Find Highly Interpretable Features in Language Models"
> Also: Bricken et al. (2023), "Towards Monosemanticity" — Anthropic
