# Mitigation Strategies After Audit

After audit, mitigation strategies become more targeted, technical, diverse and effective with greater levels of access:

| Stage | Explainability | Robustness | Fairness/Bias | Privacy |
|-------|---------------|------------|---------------|---------|
| Data and task setup | Dictionary of variables and datasheets | Collecting targeted data, reframing loss function | Alternative data sources | Anonymization |
| Feature pre-processing | Avoiding excessive feature engineering | Feature squeezing | Synthetic data | Dimensionality reduction |
| Model selection | By-design interpretable models | Adversarial training | Counterfactual fairness | Federated learning |
| Post-processing and reporting | LIME, SHAP | High confidence predictions and confidence intervals | Calibrated odds | Model inversion mitigation |
| Productionizing and deploying | Recourse interface | 'Circuit-breaking' | Monitoring panels | Rate-limiting and user's queries management |
