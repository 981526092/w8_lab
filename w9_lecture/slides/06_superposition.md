# The Problem of Superposition

## The Puzzle:
- Neural networks represent **more features than they have neurons**
- A model with 512-dimensional hidden layers may encode thousands of distinct concepts
- How? Through **superposition** — features are stored as overlapping, non-orthogonal directions

## Concrete example — a polysemantic neuron:
- In GPT-2, one neuron fires for both **"academic citations"** and **"dollar amounts"**
- Why? Both involve numbers/punctuation patterns, but rarely appear in the same context
- The model exploits this: features that rarely co-occur can **safely share a neuron**

## Analogy:
> Superposition is like **sharing seats at a party** for people who never attend together. If Alice only comes to Friday parties and Bob only comes to Saturday parties, they can share the same chair — but if both show up, there's a collision.

## The Superposition Hypothesis (Elhage et al., 2022):
- Models store features in superposition when there are **more features than dimensions**
- The degree of superposition depends on feature **sparsity** and **importance**
- Sparser features are easier to store in superposition (less collision risk)

## Why this matters:
- Individual neurons are **polysemantic** → interpreting single neurons is unreliable
- We need methods to **decompose** superposition into individual features → SAEs (next slide)

> Reference: Elhage et al. (2022), "Toy Models of Superposition" — Anthropic
