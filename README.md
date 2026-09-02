# Generative AI with Large Language Models — Lab Work

Lab work for the Coursera course [**Generative AI with Large Language Models**](https://www.coursera.org/learn/generative-ai-with-llms), offered by DeepLearning.AI and AWS.

This repo keeps the 3 hands-on labs from the course organized, documented, and version-controlled in one place.

---

## 📚 Course Overview

A 3-week hands-on course covering the generative AI project lifecycle: scoping a use case, selecting a model, prompt engineering, fine-tuning (full & parameter-efficient), evaluation, and aligning models with human feedback (RLHF).

## 📁 Repo Structure

```
genai-llms-course/
├── lab1-summarization-prompting/
├── lab2-fine-tuning-peft/
├── lab3-rlhf-detoxify/
├── requirements.txt
├── LICENSE
└── README.md
```

Each lab folder contains:
- `notebooks/` — the Jupyter notebook(s) for that lab
- `notes/` — personal notes / summary of what was learned
- `images/` — diagrams or screenshots referenced in notes
- its own `README.md` with a short summary and how to run it

## 🧪 Labs

| Lab | Topic | Key Concepts |
|-----|-------|---------------|
| [Lab 1](./lab1-summarization-prompting) | Dialogue summarization with prompt engineering | Zero-shot / one-shot / few-shot inference, generative configuration parameters |
| [Lab 2](./lab2-fine-tuning-peft) | Fine-tuning FLAN-T5 for dialogue summarization | Full fine-tuning vs. PEFT (LoRA), ROUGE evaluation |
| [Lab 3](./lab3-rlhf-detoxify) | Fine-tuning with RLHF | Reward models, PPO, reducing toxicity in generated summaries |

## 🛠️ Setup

```bash
git clone https://github.com/<your-username>/genai-llms-course.git
cd genai-llms-course
python -m venv venv
source venv/bin/activate   # on Windows: venv\Scripts\activate
pip install -r requirements.txt
```

Each lab may have its own additional `requirements.txt` if its dependencies differ (e.g., `trl`, `peft`, `evaluate`).

## 🎓 Course Certificate

[![Coursera Certificate](https://img.shields.io/badge/Coursera-Certificate-blue)](https://coursera.org/verify/J1P5Z94NA7VS)

- **Verify:** [coursera.org/verify/J1P5Z94NA7VS](https://coursera.org/verify/J1P5Z94NA7VS)
- **Share link:** [coursera.org/share/f5b699c12e03246c0c68c49d5cae757e](https://coursera.org/share/f5b699c12e03246c0c68c49d5cae757e)
- **Completed:** Aug 31, 2026
- **PDF:** [certificate.pdf](./certificate.pdf)

## 📌 Notes

- Notebooks were originally run on the AWS/Vocareum lab environment provided by the course. Some cells (e.g., pre-provisioned S3 paths) are adapted here to run locally or on Colab where possible.
- This repository is for personal learning/reference use, in line with Coursera's academic honesty policies — please don't copy this for graded submissions.

## 📄 License

MIT — see [LICENSE](./LICENSE).
