# Qwen2.5-Coder-1.5B Deep Instruction Tuning

## Project Overview
This repository contains the fine-tuning scripts, logs, and evaluation results for the **Qwen/Qwen2.5-Coder-1.5B-Instruct** model. The model was fine-tuned using LoRA (Low-Rank Adaptation) on the **Naholav/CodeGen-Deep-5K** dataset to enhance its code generation and complex instruction-following capabilities.

## Repository Structure
- `scripts/`: Python scripts used for training and evaluation.
- `logs/`: Training logs (loss values) and visualization charts.
- `report/`: A detailed PDF summary of hyperparameters and results.

## Model Details
- **Base Model:** Qwen/Qwen2.5-Coder-1.5B-Instruct
- **Dataset:** Naholav/CodeGen-Deep-5K
- **Method:** LoRA (PEFT)
- **HuggingFace Model Card:** [sinem02/qwen25-coder-1.5b-Deep]

## Training Configuration
The model was trained with the following logging configuration as per requirements:
- **Training Loss:** Logged every **20 steps**.
- **Validation Loss:** Logged every **100 steps**.

## Results
- **Final Train Loss:** [0.07]
- **Final Validation Loss:** [0.12]
- **Test Loss:** [0.17]

## How to Run
```bash
pip install -r requirements.txt
python scripts/train.py
