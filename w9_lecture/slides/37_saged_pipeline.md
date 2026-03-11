# SAGED: A Holistic Bias-Benchmarking Pipeline

> Guan, Wu et al. "SAGED: A Holistic Bias-Benchmarking Pipeline for Language Models with Customisable Fairness Calibration." **COLING 2025 Main Oral**.

## Five Modules:

```
┌─────────┐   ┌──────────┐   ┌──────────┐   ┌─────────┐   ┌──────────┐
│ SCRAPE  │──▶│ ASSEMBLE │──▶│ GENERATE │──▶│ EXTRACT │──▶│ DIAGNOSE │
│         │   │          │   │          │   │         │   │          │
│Wikipedia│   │QA or     │   │LLM +     │   │Sentiment│   │Summary   │
│Local    │   │Sentence  │   │Prompt    │   │Toxicity │   │Statistics│
│Synthetic│   │Continuat.│   │Templates │   │Regard   │   │Disparity │
└─────────┘   └──────────┘   └──────────┘   └─────────┘   └──────────┘
     ▼                                            ▼              ▼
 Any demographic                           7 feature      Impact Ratio
   concepts                               measurements   Range of Mean
```

### 1. Scrape — Collect materials from **local articles, Wikipedia, or synthetic articles**
### 2. Assemble — Build benchmarks: **Question Answering** or **Sentence Continuation**
### 3. Generate — Feed benchmarks to **LLMs** with prompt templates, collect responses
### 4. Extract — Measure: **sentiment, regard, personality, toxicity, stereotype, baseline distance, cluster distance**
### 5. Diagnose — Compute **summary statistics**, apply **comparison functions**, output **disparity metrics**

## Key Innovation — Fairness Calibration:
- **Baseline Calibration**: G(x, f_calibrated) = G(x, f) - G(baseline, f) — cancels out bias in questions and metric tools
- **Counterfactual Branching**: Ensures prompts are comparable across concepts
