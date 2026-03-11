# Summary

## Mechanistic Interpretability:
- **Linear probes** reveal what information is encoded at each layer
- **Superposition** explains why individual neurons are polysemantic
- **Sparse autoencoders** decompose superposition into interpretable monosemantic features
- **Activation patching** identifies which components cause specific behaviors
- **Neuronpedia** provides an interactive platform for exploring SAE features

## Human-in-the-Loop AI:
- **Active Learning:** model-driven, human as oracle for labelling
- **Interactive ML:** shared control, bidirectional human-model feedback
- **Machine Teaching:** human-driven curriculum design for models
- LLM training (pre-training → SFT → RLHF) is a real-world example of HITL at every stage

## AI Auditing & Governance:
- Algorithm audits assess **efficacy, robustness, fairness, transparency, and privacy**
- The audit cycle: **Development → Assessment → Mitigation → Assurance**
- **EU AI Act**: Risk-based classification, GPAI obligations, penalties up to €35M/7%
- **NYC Local Law 144**: Bias audits for automated employment decision tools

## AI Bias:
- Bias can be introduced at **every stage** of the LLM lifecycle
- **Intrinsic** (WEAT, CrowS-Pairs) vs **Extrinsic** (BOLD, SAGED, BBQ, JobFair) detection
- **SAGED** pipeline: holistic benchmarking with fairness calibration
- Fairness calibration (baseline + counterfactual branching) essential for accurate measurement
