# Lab 2 — Fine-Tune a Generative AI Model for Dialogue Summarization

## Goal
Improve on prompting alone by actually fine-tuning FLAN-T5 on the summarization task, and compare full fine-tuning vs. parameter-efficient fine-tuning (PEFT).

## What this lab covers
- Preparing the `DialogSum` dataset for instruction fine-tuning
- **Full fine-tuning** of FLAN-T5 and evaluating with ROUGE metrics
- **PEFT with LoRA** (Low-Rank Adaptation) — training a small number of additional parameters instead of the full model
- Comparing human-quality evaluation and ROUGE scores across: original model → full fine-tuned → PEFT/LoRA fine-tuned
- Discussing the trade-offs: training cost/memory vs. performance

## Files
- `notebooks/Lab_2_fine_tune_generative_ai_model.ipynb` — main notebook
- `notes/summary.md` — my takeaways

## How to run
```bash
pip install -r requirements.txt
jupyter notebook notebooks/Lab_2_fine_tune_generative_ai_model.ipynb
```

## Key takeaway
LoRA gets close to full-fine-tuning ROUGE scores while training a tiny fraction of the parameters — a much better cost/performance trade-off for most practical use cases.
