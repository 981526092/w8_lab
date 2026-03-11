# Is Transparency Useful?

Post-hoc explanations don't just describe a model — they let us **falsify** its reasoning.

## Scrutiny: Exposing spurious correlations
- A model classified huskies as "wolf" with high confidence
- Saliency maps revealed it relied on **snow in the background**, not the animal
- Without xAI, the model's accuracy alone looked fine (Ribeiro et al. 2016)

## Vulnerability detection: Adversarial robustness
- Adversarial stickers on a **stop sign** caused a model to predict "Speed Limit 45"
- xAI methods can reveal that the model attends to **fragile, easily manipulated features** (Eykholt et al. 2018)

## Takeaway
- High accuracy ≠ correct reasoning
- xAI lets us **audit** what a model has actually learned — catching problems that test-set metrics miss
