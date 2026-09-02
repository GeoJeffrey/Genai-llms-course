# Lab 1 — Generative AI Use Case: Dialogue Summarization with Prompt Engineering

## Goal
Explore how the input (prompt) to a large language model affects the output, using dialogue summarization as the example task.

## What this lab covers
- Loading the FLAN-T5 model and the `DialogSum` dataset
- Summarizing dialogue **without prompt engineering** (baseline)
- **Zero-shot inference** with a plain prompt
- **Zero-shot inference with an instruction prompt template**
- **One-shot** and **few-shot inference** by including example dialogue/summary pairs in the prompt
- Tuning generative configuration parameters (`max_new_tokens`, `do_sample`, `temperature`, etc.) and observing their effect on output

## Files
- `notebooks/Lab_1_summarize_dialogue.ipynb` — main notebook
- `notes/summary.md` — my takeaways

## How to run
```bash
pip install -r requirements.txt
jupyter notebook notebooks/Lab_1_summarize_dialogue.ipynb
```

## Key takeaway
Few-shot prompting with well-chosen examples generally improves summary quality over zero-shot, but returns diminish after ~3–5 examples, and results are still highly sensitive to prompt wording.
