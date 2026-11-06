# 🤖 LLM Evaluation: 10 Models, 70 Questions

![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![Models](https://img.shields.io/badge/Models-10-8A5CC2)
![Questions](https://img.shields.io/badge/Questions-70-3CB043)

How reliable are today's popular AI models? This project compares **ChatGPT, Gemini, Claude, LLaMA 3, Mistral, Falcon, Perplexity, Grok, DeepSeek and Gemma** on the same 70 questions and measures them with Accuracy, Precision, Recall, Bias and Hallucination Rate. Run the notebook to see the full results, charts and heatmap.

---

## 📁 Files

| File | What it contains |
|---|---|
| `paper_final.ipynb` | Full analysis: data cleaning, metrics, charts and heatmap |
| `models.csv` | Ground Truth and the TRUE/FALSE verdict of each model (70 rows) |
| `llm_eval_questions.xlsx` | Question text, model answers, benchmark answer and reference link |

---

## 📏 Metrics

| Metric | Formula | In simple words |
|---|---|---|
| Accuracy | (TP + TN) / N | How often the model is right overall |
| Precision | TP / (TP + FP) | When it says TRUE, how often it is correct |
| Recall | TP / (TP + FN) | How many real TRUE cases it finds |
| Bias | \|predicted TRUE − actual TRUE\| / N | How much it leans to TRUE or FALSE |
| Hallucination Rate | FP / (TP + FP) × 100 | Share of its TRUE answers that are wrong |

---

## ▶️ How to Run

```bash
pip install pandas numpy matplotlib jupyter
jupyter notebook paper_final.ipynb
```