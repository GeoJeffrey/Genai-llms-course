# Lab 3 — Fine-Tune FLAN-T5 with Reinforcement Learning (RLHF) to Generate Less-Toxic Summaries

## Goal
Use Reinforcement Learning from Human Feedback (RLHF) to align the fine-tuned model's outputs with a human preference — in this case, generating less toxic/more positive summaries.

## What this lab covers
- Using Meta AI's hate-speech **reward model** as a proxy for human feedback
- Setting up **Proximal Policy Optimization (PPO)** with the `trl` library to fine-tune the PEFT model from Lab 2
- Evaluating toxicity before vs. after RLHF fine-tuning, quantitatively and qualitatively
- Discussing reward hacking and the challenges of aligning LLMs with human values

## Files
- `notebooks/Lab_3_fine_tune_model_to_detoxify_summaries.ipynb` — main notebook
- `notes/summary.md` — my takeaways

## How to run
```bash
pip install -r requirements.txt
jupyter notebook notebooks/Lab_3_fine_tune_model_to_detoxify_summaries.ipynb
```

## Key takeaway
RLHF measurably reduces toxicity scores on held-out summaries, but requires careful reward model choice — a poorly matched reward model can push outputs to be vague or evasive rather than genuinely better.
