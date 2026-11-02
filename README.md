# Practical LLM Fine-Tuning

A hands-on implementation exploring the complete LLM fine-tuning workflow using Hugging Face, PEFT, LoRA, QLoRA, and Unsloth.

## Tech Stack
- Python
- PyTorch
- Hugging Face Transformers
- PEFT
- LoRA and QLoRA
- BitsAndBytes
- Unsloth
- TRL

## Model
Qwen/Qwen2.5-0.5B-Instruct

## Dataset
[FinQA](https://github.com/czyssrs/FinQA) — a financial question-answering dataset containing numerical reasoning problems.

| Split | Examples |
|---|---:|
| Training | 6,251 |
| Validation | 883 |
| Testing | 1,147 |

## Work Completed
- Hugging Face model loading and inference
- Parameter-efficient fine-tuning using LoRA
- 4-bit quantization using QLoRA
- Model optimization using Unsloth
- Dataset preparation and tokenization
- Prompt-completion formatting
- Training and validation
- Loss masking and completion-preservation audits
- Training and validation loss analysis

## Training Experiment

- Epochs: 2
- Training steps: 1,564
- Trainable parameters: 4,399,104 (0.88%)
- Final training loss: 1.184976
- Final validation loss: 1.393749

## Limitations

The corrected training run completed successfully, but its adapter weights were not persisted before the Kaggle session ended.

Consequently, the final corrected model could not undergo a complete benchmark evaluation. Earlier experimental evaluation results are not treated as reliable benchmark measurements.

## Learning Outcome

Developed practical understanding of parameter-efficient fine-tuning, quantization, dataset preparation, training objectives, loss masking, and model evaluation workflows.
