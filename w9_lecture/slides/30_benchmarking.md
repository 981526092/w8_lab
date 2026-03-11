# Quantitative Assessment — Benchmarking

## What is benchmarking?
- A success-testing intervention that assesses an AI system's performance against a predefined task
- Can be deployed throughout model development for iteratively improving model efficacy ("hill-climbing")

## What benchmarks measure:
- **Efficacy:** aggregate benchmarks (MMLU), comprehension (HellaSwag), math (MATH), factuality (FACTOR)
- **Model harms:** representational biases (BOLD, BBQ), mis/disinformation (FEVER), toxicity (ToxiGen)
- Used to compare relative efficacy with other models, or a model's different development iterations

## Limitations of benchmarking:
- Lack of fit-for-purpose benchmarks across model harms and modalities
- Risks of **memorisation** — model inadvertently training on public benchmarks, reducing accuracy
- **Resource intensive**, requiring significant tooling support
- **Capability overhang:** Over-reliance on benchmarks may lead to unknown risks being ignored
