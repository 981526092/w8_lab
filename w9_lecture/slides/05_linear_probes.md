# Linear Probes

## What are Linear Probes?
- A technique to test **what information is encoded** in a model's internal representations
- Train a simple **linear classifier** on top of a hidden layer's activations
- If the probe achieves high accuracy, the information is **linearly accessible** in that layer

## How it works:
1. Run inputs through the model, extract activations at a specific layer
2. Freeze the model weights — only train a linear layer on top
3. Evaluate: can this linear layer predict the property of interest?

## Concrete Example — Probing for Factual Knowledge:
- Input: "The Eiffel Tower is located in ___"
- Extract activations from each layer of GPT-2
- Train a linear probe to predict the answer entity ("Paris") from each layer's activations
- Result: Early layers (~1-5) encode syntax → Middle layers (~6-12) encode semantic/factual info → Final layers produce the output
- Probing accuracy **increases sharply** at middle layers, showing factual knowledge is concentrated there

## Another Example — Probing for Sentiment:
- Feed movie reviews into BERT, extract layer activations
- Train linear probe to classify positive vs negative sentiment
- If layer 8 achieves 95% accuracy but layer 2 only 60% → sentiment representation **emerges gradually** through the network

## Key insight:
- Linear probes help us map **where** specific information lives in the network
- Limitation: a successful probe shows information is *present*, not necessarily that the model *uses* it

> Reference: Alain & Bengio (2017), "Understanding intermediate layers using linear classifier probes"
