# LaTeX Image Translation with Vision-Language Models

This repository contains my implementation of **LaTeX Image Translation** using state-of-the-art **Vision-Language Models (Qwen2-VL, LLaVA)**.  
The goal of this project is to translate mathematical equation images into corresponding LaTeX code with high accuracy and efficiency.


## Project Overview
- **Dataset**: [LaTeX-OCR dataset] (~76k image–LaTeX pairs)
- **Models Used**: 
  - Qwen2-VL
  - LLaVA-1.5
- **Fine-Tuning Approach**:
  - **LoRA (Low-Rank Adaptation)** for Parameter-Efficient Fine-Tuning
  - **4-bit quantization**  for memory-efficient training
  - **Gradient checkpointing** and **mixed precision** for scalability


## Key Results
- Achieved **BLEU score: 0.73** and **ROUGE-L F1: 0.70**
- Outperformed LLaVA-1.5 baselines on LaTeX-OCR benchmark
- Demonstrated effectiveness of **lightweight fine-tuning** for math-aware OCR
- Trained efficiently on **consumer GPUs**


## Repository Structure
- `Finetuning_QwenVL_updated.ipynb` – Jupyter notebook with full training + evaluation pipeline
- `README.md` – Project documentation 

