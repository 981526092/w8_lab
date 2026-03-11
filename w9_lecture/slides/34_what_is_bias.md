# What is Bias?

## Real-world examples:
- **Amazon (2018):** Internal AI recruiting tool penalised resumes containing the word "women's" (e.g., "women's chess club captain") — trained on 10 years of male-dominated hiring data
- **COMPAS:** Criminal risk assessment tool scored Black defendants as higher risk than White defendants with similar profiles
- **Google Photos (2015):** Image classifier labelled photos of Black people as "gorillas"

## Bias appears at multiple levels:
- **Human Bias:** Cognitive shortcuts — e.g., associating "nurse" with "female"
- **Algorithmic Bias:** Model amplifies patterns in biased training data
- **LLM Bias:** Language models inherit stereotypes from internet text corpora

## Individual vs Group Fairness:

| | Individual Fairness | Group Fairness |
|---|---|---|
| **Definition** | Similar individuals treated similarly | Demographic groups receive similar outcomes |
| **Example** | Two identical resumes → same score regardless of name | Male and female candidates → similar selection rates |
| **Challenge** | Defining "similarity" | May conflict with individual fairness |

> These two can conflict: promoting group fairness (equal selection rates) may require treating similar individuals differently
