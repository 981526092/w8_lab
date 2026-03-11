# Ingredients of the Development Process

Documentation created as part of the algorithm-building phases are essential for (internal/external) risk mapping. Two key documents:

## Model Cards:
- **Model Details:** Core information about the AI model (origin, version, technical specifics)
- **Intended Use:** Primary applications and target audience; scenarios it's not suited for
- **Factors:** Variables (demographics, environmental conditions) that may influence performance
- **Metrics:** Measures and criteria used to evaluate effectiveness
- **Evaluation Data:** Datasets used for assessing the model
- **Training Data:** Data used to train the model
- **Quantitative Analyses:** Numerical findings from testing (standalone and intersectional metrics)
- **Ethical Considerations:** Ethical aspects and potential biases
- **Caveats and Recommendations:** Warnings and advice for deployment

## Example — GPT-4 Model Card (excerpt):
- **Model Details:** Autoregressive transformer, OpenAI, March 2023
- **Intended Use:** General-purpose assistant; NOT for medical diagnosis or legal advice
- **Factors:** Performance varies by language (English >> others), topic domain, prompt style
- **Metrics:** MMLU 86.4%, HumanEval 67%, HellaSwag 95.3%
- **Ethical Considerations:** Can generate harmful content; RLHF mitigations applied

## Data Sheets:
- **Motivation** → **Composition** → **Collection Process** → **Preprocessing/cleaning/labeling** → **Uses** → **Distribution** → **Maintenance**
