# Key Components of Algorithm Auditing — 1

## The audit cycle has four phases:
1. **Development** — Data, Pre-processing, Modelling, Post-processing, Production
2. **Assessment** — Robustness, Explainability, Privacy, Bias
3. **Mitigation** — Surrogate Explanations, Anonymization, Synthetic data
4. **Assurance** — Risk rating, Certification, Best practices, Insurance

## Running example — auditing a hiring algorithm:

| Phase | What happens |
|-------|-------------|
| **Development** | Company trains a resume-screening model on 5 years of hiring data |
| **Assessment** | Auditors test for **disparate impact** — find the model rejects female applicants at 2x the rate |
| **Mitigation** | Apply **counterfactual fairness**: would the decision change if gender-correlated features were swapped? Retrain with debiased embeddings |
| **Assurance** | System certified under **NYC Local Law 144** — annual bias audit published, candidates notified of AI use |

## Object of audit:
- Algorithms (data + model + development process + documentation)

## What to audit — development stages vs risk verticals:

| Stage | Explainability | Robustness | Fairness/Bias | Privacy |
|-------|---------------|------------|---------------|---------|
| Data and task setup | Data collection and labelling | Data accuracy | Population balance | DPIA |
| Feature pre-processing | Dictionary of variables | Feature engineering | Fair representations | Data minimization |
| Model selection | Model complexity | Model validation | Fairness constraints | Differential privacy |
| Post-processing and reporting | Auxiliary tools | Adversarial testing | Bias metric assessment | Model inversion |
| Productionizing and deploying | Interface and documentation | Concept drift detection and CI | Real-time monitoring of bias metrics | Rate-limiting and user's queries management |
