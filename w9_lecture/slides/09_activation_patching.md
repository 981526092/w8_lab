# Activation Patching

## What is Activation Patching?
- A **causal intervention** technique to identify which components of a model are responsible for a specific behavior
- Also known as **causal tracing** or **interchange interventions**

## How it works:

```
Clean run:    "The Eiffel Tower is in ___"
              ┌──────┐  ┌──────┐  ┌──────┐
              │ L1   │─▶│ L5*  │─▶│ Lout │──▶ "Paris" ✓
              └──────┘  └──────┘  └──────┘

Corrupted:    "The Colosseum is in ___"
              ┌──────┐  ┌──────┐  ┌──────┐
              │ L1   │─▶│ L5   │─▶│ Lout │──▶ "Rome"
              └──────┘  └──────┘  └──────┘

Patched:      "The Colosseum is in ___"  + patch L5* from clean
              ┌──────┐  ┌──────┐  ┌──────┐
              │ L1   │─▶│ L5*  │─▶│ Lout │──▶ "Paris" ✓
              └──────┘  └──────┘  └──────┘
                         ▲ patched!
→ L5 was critical for storing "Eiffel Tower → Paris"
```

## What can be patched:
- Individual **attention heads**, **MLP layers**, **residual stream**, individual **SAE features**

## Key applications:
- **Localizing** where factual knowledge is stored
- Understanding **circuit-level** computation (e.g., "induction heads" for in-context learning)
- Debugging **failure modes** — which component causes a wrong answer?

> Reference: Meng et al. (2022), "Locating and Editing Factual Associations in GPT"
> Also: Wang et al. (2023), "Interpretability in the Wild"
