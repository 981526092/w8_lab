# The AI Development Pipeline & Why Humans Are in the Loop

## The 7 stages of ML development:
1. **Defining Objectives** → 2. **Gathering Data** → 3. **Data Preparation** → 4. **Model Selection** → 5. **Training** → 6. **Validation & Testing** → 7. **Deployment & Maintenance**

## Humans are critical at every stage — concrete example (medical AI):

| Stage | What the human does |
|-------|-------------------|
| Objectives | Clinicians define: "detect pneumonia from chest X-rays" |
| Data | **Radiologists label** 100k X-rays as normal/abnormal |
| Preparation | Experts verify labels, remove duplicates, balance classes |
| Model selection | Engineers choose CNN architecture suited to imaging |
| Training | Monitor for overfitting, adjust hyperparameters |
| Validation | **Clinicians verify** accuracy on held-out cases — catch false negatives |
| Deployment | Ongoing monitoring: does performance degrade on new scanner hardware? |

## Why investigate Human-in-the-Loop ML?
- To make machine learning **more powerful** (human expertise fills gaps in data/labels)
- To make humans **more effective and efficient** (AI handles volume, humans handle judgment)
- This falls under **Human-in-the-Loop ML (HITL-ML)** — our focus for the next several slides

> Key reference: Mosqueira-Rey et al. (2023) — https://doi.org/10.1007/s10462-022-10246-w
