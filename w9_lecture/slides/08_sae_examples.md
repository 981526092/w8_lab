# SAE Features in Practice

## What do SAE features look like?

### Example features found in language models:
- A feature that activates on **Python f-strings**
- A feature that activates on **references to the Golden Gate Bridge**
- A feature that activates on **expressions of hedging/uncertainty** ("maybe", "perhaps", "it's possible")
- A feature that activates on **base64-encoded text**
- A feature that activates on **legal contract language**

## Feature steering:
- By **artificially activating** a specific SAE feature, we can steer model behavior
- Famous example: Anthropic's "Golden Gate Claude" — amplifying the Golden Gate Bridge feature caused Claude to constantly reference the bridge

## Why SAEs matter for safety:
- Enable understanding of **what concepts models have learned**
- Help detect **undesirable features** (deception, bias, harmful content patterns)
- Provide a path toward **fine-grained control** of model behavior

> Anthropic (2024): "Scaling Monosemanticity: Extracting Interpretable Features from Claude 3 Sonnet"
