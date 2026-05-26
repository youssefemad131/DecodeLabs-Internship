# 🚀 DecodeLabs AI Engineering Internship
### Batch 2026 | Industrial Training Kit

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-In%20Progress-blue?style=for-the-badge)



## 🗂️ Repository Structure

```
📦 DecodeLabs-Internship/
│
├── 📁 Project 1/
│   ├── 📁 Code/
│   │   └── 📓 rule_based_chatbot.ipynb
│   └── 📄 README.md
│
├── 📁 Project2/
│   ├── 📁 code/
│   │   └── 📓 iris_classification_knn.ipynb
│   └── 📄 README.md
│
├── 📁 Project 3/
│   ├── 📁 Code/
│   │   ├── 📓 Project3_AI_Recommendation.ipynb
│   │   └── 📊 glassdoor_jobs.csv
│   └── 📄 README.md
│
└── 📄 README.md  ← You are here
```

---

## 📋 Projects Overview

### 🤖 Project 1 — Rule-Based AI Chatbot
> **Phase:** Foundation | **Type:** Deterministic AI | **Concept:** White Box System

Build a rule-based chatbot (DecoBot) from scratch using pure Python — no ML, no neural networks. Master control flow, decision-making logic, and the IPO model before touching any machine learning.

| | |
|---|---|
| **Key Concepts** | Control flow, if-else logic, dictionary O(1) lookup, infinite loop, input sanitization |
| **Tech Stack** | Python, `random`, `datetime` |
| **Architecture** | IPO Model — Input (Sanitization) → Process (Intent Matching) → Output (Response) |
| **Highlight** | Dictionary-based lookup is ~100x faster than if-elif ladders at scale |

---

### 🌸 Project 2 — Data Classification Using AI
> **Phase:** Predictive | **Type:** Supervised Learning | **Algorithm:** K-Nearest Neighbors

Build a complete KNN classifier on the Iris dataset — covering the full ML pipeline from raw data exploration to validated model predictions.

| | |
|---|---|
| **Key Concepts** | Feature scaling, train-test split, KNN, confusion matrix, F1 score, elbow method |
| **Tech Stack** | Python, Scikit-learn, Pandas, Matplotlib, Seaborn |
| **Dataset** | Iris — 150 samples, 3 classes (Setosa, Versicolor, Virginica), 4 features |
| **Highlight** | Elbow Method to find optimal K + decision boundary visualization |

---

### 🎯 Project 3 — AI Recommendation Logic
> **Phase:** Intelligent Systems | **Type:** Content-Based Filtering | **Algorithm:** TF-IDF + Cosine Similarity

Build an AI-powered job recommendation engine using 956 real Glassdoor job postings. The system maps user skills to job roles using TF-IDF vectorization and Cosine Similarity — no neural networks, pure algorithmic logic.

| | |
|---|---|
| **Key Concepts** | Content-based filtering, TF-IDF, cosine similarity, vector space model, cold start |
| **Tech Stack** | Python, Scikit-learn, Pandas, Matplotlib, Regex |
| **Dataset** | Glassdoor Jobs (Kaggle) — 956 postings, 328 unique titles, 63 industries |
| **Highlight** | TF-IDF matrix of 848 × 625 terms; rare skills (pytorch, kubernetes) scored higher than generic ones |

---

## 📈 Learning Progression

```
Project 1               →         Project 2               →         Project 3
────────────────────              ────────────────────              ────────────────────
Rule-Based Logic                  Supervised Learning               Recommendation AI
Deterministic                     Probabilistic                     Similarity-Based
dict lookup  O(1)                 KNN Algorithm                     Cosine Similarity
No training data                  Iris Dataset (150 rows)           Glassdoor (956 jobs)
Control Flow                      Model Evaluation                  Content Filtering
Exact key → value                 Feature vector → class            Skill vector → job role
```

---

## 🛠️ Tech Stack

| Tool | Used In |
|------|---------|
| Python 3.8+ | All Projects |
| Jupyter Notebook | All Projects |
| Scikit-learn | Project 2, 3 |
| Pandas & NumPy | Project 2, 3 |
| Matplotlib & Seaborn | Project 2, 3 |
| Regex (`re`) | Project 3 |

---
## 📌 About This Repository

This repository documents my journey through the **DecodeLabs AI Engineering Internship — Batch 2026**. Each project is a hands-on milestone that builds on the last — starting from pure logic and control flow, progressing through supervised learning, and into intelligent recommendation systems.

> *"The absolute best way to master Artificial Intelligence is through hands-on practice, not just theory."* — DecodeLabs

---
---

## 👨‍💻 About Me

**Youssef Emad Samouel**
AI & Machine Learning Engineer | Computer Science Student — AI Department

I'm a Computer Science student at Benha University (GPA 3.7/4.0) specializing in Artificial Intelligence, with hands-on experience building and deploying ML and NLP systems. I've completed 330+ hours of advanced AI training through NVIDIA DLI, NTI, and ITI, and delivered 5+ real-world projects across NLP, Computer Vision, and ML.

Currently interning at **DecodeLabs** as an AI/ML Engineer, where I develop and benchmark ML models, preprocess large-scale datasets, and document reproducible research workflows.

**🔧 Core Skills**
- **AI/ML:** Scikit-learn, TensorFlow, PyTorch, Keras, Hugging Face Transformers
- **NLP:** spaCy, NLTK, TF-IDF, Text Classification, Sentiment Analysis, NER
- **Data:** Pandas, NumPy, Matplotlib, Seaborn, Power BI
- **Dev Tools:** Git, GitHub, Streamlit, Gradio, Google Colab

**🏆 Highlights**
- 93%+ accuracy on Plant Disease Detection (CNN, 30,000+ images)
- 88%+ accuracy on IMDB Sentiment Analysis (50,000 reviews, live Gradio demo)
- ACO path-planning algorithm outperformed alternatives by 25% across 10+ environments

[![LinkedIn](https://img.shields.io/badge/LinkedIn-youssef--emad1312-0A66C2?style=flat&logo=linkedin)](https://linkedin.com/in/youssef-emad1312)
[![GitHub](https://img.shields.io/badge/GitHub-youssefemad131-181717?style=flat&logo=github)](https://github.com/youssefemad131)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-6C47FF?style=flat&logo=vercel)](https://youssef-emad-portfolio.lovable.app)

---


## 🏢 About DecodeLabs

DecodeLabs is an industrial training organization based in Greater Lucknow, India, focused on building real-world AI engineering skills through hands-on project-based learning.

 ✉️ decodelabs.tech@gmail.com | 🌐 [www.decodelabs.tech](http://www.decodelabs.tech)

---

*Built with 💻 and ☕ — DecodeLabs AI Industrial Training Kit | Batch 2026*
