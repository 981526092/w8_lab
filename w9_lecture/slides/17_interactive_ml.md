# Interactive Machine Learning (IML)

## Definition:
- **Control is shared** between human and model — bidirectional feedback via an interface
- Humans perform more tasks beyond labelling: correcting, guiding, adjusting features

## How it differs from Active Learning:
- AL: model controls, human just labels → IML: **human and model collaborate** iteratively
- HCI design is critical — the interface shapes the learning outcome

## Concrete Example — Interactive Image Segmentation:
- Task: Segment tumours in MRI scans
- Model makes initial segmentation → Radiologist **corrects boundaries** directly on the interface → Model updates in real-time → Radiologist refines again
- Unlike AL (where the doctor only labels "tumour/no tumour"), the doctor actively **shapes** the model's understanding by drawing corrections
- Result: Both the model improves AND the doctor works faster with each iteration

## Limitations:
- Depends on **presence of human experts** throughout the process
- Must deal with human limitations: attention fatigue, inconsistency, availability
- ML and HCI aspects must be carefully **intermingled**
