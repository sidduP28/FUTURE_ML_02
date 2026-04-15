# FUTURE_ML_02
# IT Support Ticket Classifier

> Automatically classify IT support tickets by **type** and **priority** using NLP and machine learning — reducing manual triage effort and improving response time.

---

## 📌 Project Overview

It is an NLP-powered classification system that processes raw IT helpdesk tickets and predicts:
- **Ticket Type** — e.g., Hardware, Software, Network, Access
- **Ticket Priority** — e.g., Low, Medium, High, Critical

It uses **TF-IDF vectorization** paired with **Logistic Regression** and **Random Forest** pipelines, achieving **86% accuracy on ticket type** and **83% on priority**.

---

## 🗂️ Dataset

| Field | Description |
|-------|-------------|
| `ticket_text` | Raw text of the support ticket |
| `ticket_type` | Category label (target 1) |
| `priority` | Priority label (target 2) |

> Dataset source: [mention Kaggle/synthetic/internal source here]

---

## ⚙️ Tech Stack

![Python](https://img.shields.io/badge/Python-3.10-blue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3-orange)
![Pandas](https://img.shields.io/badge/Pandas-2.0-green)

- **Text Preprocessing** — Lowercasing, regex cleaning, stopword removal (NLTK)
- **Vectorization** — TF-IDF (`TfidfVectorizer`)
- **Models** — Logistic Regression, Random Forest Classifier
- **Pipeline** — `sklearn.pipeline.Pipeline` for clean train/test flow
- **Evaluation** — Accuracy, Classification Report, Confusion Matrix

---

## 🏗️ Project Structure

```
AutoTriage/
│
├── IT_helpdesk_Ticket_Classification.ipynb  # Main notebook
├── data/
│   └── tickets.csv                          # Dataset
└── README.md
```

---

## 📊 Results

| Task | Model | Accuracy |
|------|-------|----------|
| Ticket Type | Logistic Regression | **86%** |
| Ticket Priority | Random Forest | **83%** |

---

## 🔍 Key Learnings

- TF-IDF effectively captures domain-specific vocabulary in ticket text
- Logistic Regression generalizes better than Random Forest for multi-class text classification on small datasets
- Separate pipelines for each target (type vs priority) outperforms a single multi-output model

---

## 👤 Author

**Siddartha**
[LinkedIn](linkedin.com/in/pitchuka-anjani-siddartha-7a88593bb/?skipRedirect=true) ·
[Kaggle](#https://www.kaggle.com/siddartha4)
