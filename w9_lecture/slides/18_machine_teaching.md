# Machine Teaching (MT)

## Definition:
- Responsibility **firmly on the teacher** — the human designs the curriculum for the model
- The teacher can be a **human** or an **algorithm** itself

## Concrete Example — Teaching a Robot to Pour Water:
- A robotics engineer doesn't label 10,000 images of pouring (that's AL)
- Instead, they **design a curriculum**: first teach "grasp cup" → then "tilt slowly" → then "stop when full"
- The teacher decides **what to teach and in what order** — like a teacher designing a lesson plan
- The model never selects its own training data; the human expert controls the entire learning process

## Two types:

### Humans as Teachers (Interactive MT):
- Makes ML accessible to non-ML experts (e.g., AutoML, no-code ML platforms)
- Human prepares curriculum → explains knowledge → assesses model predictions

### Machines as Teachers (Iterative MT):
- A machine teacher knows the target model and designs **optimal training sets**
- Example: Determining the **Minimum Viable Dataset** — what is the smallest dataset needed to teach a concept?

## Limitations:
- Teaching with **imperfect knowledge** of the learner leads to sub-optimal curricula
- Deeper question: how can humans teach models to **surpass human capabilities**?
