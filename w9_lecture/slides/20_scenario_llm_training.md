# Scenario: How are LLMs Trained?

## The pipeline — HITL at every stage:

| Stage | What happens | Human role |
|-------|-------------|------------|
| **Data Collection & Pre-processing** | Gather and clean training data | No direct human involvement |
| **Pre-training (Self-Supervised Learning)** | Learn language patterns | Compute heavy; creates Base Model |
| **Supervised Fine-Tuning** | Train on examples of correct outputs | Similar to **Machine Teaching** — humans prepare data; creates Assistant Model |
| **RLHF (Reinforcement Learning with Human Feedback)** | Humans rank multiple model responses | Direct **HITL process** — feeds into a Reward Model; LLM is fine-tuned with RL (PPO) |
| **Post-Deployment Feedback & Continuous Learning** | User feedback and monitoring | Some human involvement; go back to fine-tuning... |
