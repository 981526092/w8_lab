# Sources of Bias in the LLM Lifecycle

## Stage 1: Pre-training Data
- **Historical bias**: Training data reflects past prejudices
- **Sampling bias**: Over/under-representation of groups
- Example: Common Crawl is ~60% English → models perform worse on non-English languages and non-Western cultural contexts

## Stage 2: Model Architecture & Training
- **Inductive bias**: Word embeddings encode stereotypes
- Example: Word2Vec famously learned "Man:Computer Programmer :: Woman:Homemaker" from Google News corpus

## Stage 3: Fine-tuning & Human Feedback
- **Human feedback bias**: RLHF annotators are often young, English-speaking, from specific demographics
- Example: If annotators from one culture rate responses, the model learns to optimise for **that culture's preferences**

## Stage 4: Evaluation & Deployment
- **Evaluation bias**: Benchmarks may miss harms for specific groups
- Example: A chatbot tested mainly in English may produce toxic content in other languages where safety training data is sparse

> Bias can be introduced or amplified at **every stage** — mitigation must be holistic
