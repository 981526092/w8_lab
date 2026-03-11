# Bias Detection in LLMs

## Intrinsic Bias (internal representations):

### Similarity-based metrics (embedding space):
- **WEAT** (Word Embedding Association Test): Measures association between concept words and attribute words in embedding space
- **SEAT** (Sentence Encoder Association Test): Extends WEAT to sentence-level embeddings
- Limitation: Hard to apply to LLMs that don't expose static embeddings

### Probability-based metrics (model outputs):
- **CrowS-Pairs**: Measures stereotypical preferences in masked token predictions
- **StereoSet**: Tests whether models prefer stereotypical over anti-stereotypical associations
- Limitation: Limited to specific templates, may not capture open-ended generation bias

## Extrinsic Bias (downstream behaviour):

### Open-ended generation:
- **BOLD** (Bias in Open-ended Language Generation): Prompts models with Wikipedia sentences about demographic groups, measures sentiment/toxicity
- **SAGED**: A holistic bias-benchmarking pipeline with customisable fairness calibration (see next slides)

### Decision tasks:
- **BBQ** (Bias Benchmark for QA): Tests stereotypical reasoning in ambiguous vs. disambiguated contexts
