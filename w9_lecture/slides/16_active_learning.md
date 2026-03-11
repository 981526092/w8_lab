# Active Learning (AL)

## Definition:
- The **system remains in control** and uses humans as oracles to annotate data
- The active learner attempts to maximise accuracy using **as few labelled instances as possible**

## Process:
1. Collect unlabeled instances → 2. Model selects most **uncertain/informative** samples → 3. Human labels them → 4. Retrain → 5. Repeat until performance is sufficient

## Concrete Example — Medical Imaging:
- Task: Classify 100,000 X-rays as "pneumonia" or "normal"
- Labelling all 100K images by radiologists is prohibitively expensive
- **Active Learning approach**: Train on 500 labelled images → model identifies the 100 X-rays it is **most uncertain** about → radiologist labels those 100 → retrain → repeat
- Result: Achieve 95% accuracy by labelling only **2,000 images** instead of 100,000 — saving months of expert time

## Limitations:
- **Noisy oracles:** How to decide an oracle label is trustworthy?
- **Variable labelling cost:** Not all labels are equally expensive to obtain
- **Cold start:** Initial model may select uninformative samples
