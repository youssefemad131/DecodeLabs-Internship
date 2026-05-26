
# 🤖 Rule-Based AI Chatbot
### Project 1 — DecodeLabs Industrial Training Kit | Batch 2026

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Type](https://img.shields.io/badge/AI%20Type-Deterministic-00C853?style=for-the-badge)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-2ea44f?style=for-the-badge)

---

## 📌 Overview

This is Project 1 of the **DecodeLabs AI Engineering Internship Track** — the foundation phase. Before building systems that learn on their own, you master the art of teaching a machine through **explicit rules and logic**.

> *"An LLM without rules is a hallucination engine. Today, we build the skeleton that holds the intelligence."*

---

## 🎯 Project Goal

Build a **Rule-Based AI Chatbot** (DecoBot) using pure Python — no machine learning, no neural networks. The chatbot simulates human conversation through deterministic control flow, dictionary-based intent matching, and a continuous input loop.

---

## 🧠 Core Concept: The Two Minds of AI

| | System 1 — The Artist | System 2 — The Engineer |
|---|---|---|
| **Type** | Probabilistic | **Deterministic** ← This project |
| **Example** | GPT, BERT, LLMs | Rule-based chatbot |
| **Output** | Creative, flexible | Exact, traceable |
| **Risk** | Hallucination | Limited vocabulary |
| **Advantage** | Handles anything | Zero hallucination, 100% auditable |

**Why it matters:** Rule-based systems are the **guardrails** that sit in front of LLMs in production — frameworks like NVIDIA NeMo and Llama Guard are built on this exact principle. You are building the control layer.

---

## 🗂️ Project Structure

```
📦 rule-based-chatbot/
├── 🐍 chatbot.py                  # Standalone Python script (run in terminal)
├── 📓 rule_based_chatbot.ipynb    # Full notebook with theory + benchmarks
├── 📄 README.md                   # This file
```

---

## ⚙️ Architecture — The IPO Model

```
INPUT                    PROCESS                   OUTPUT
─────────────────        ──────────────────────    ──────────────────────
Raw user text       →    Sanitization              →   Cleaned response
"HeLLo"                  .lower().strip()
"  HELLO  "              ↓
"hello"                  Intent Matching
                         dict.get() → O(1)
                         Partial keyword scan
                         Fallback handler
```

### The Logic Skeleton (Project Specification)

| Component | Description | Implementation |
|-----------|-------------|----------------|
| **Input Loop** | Continuous `while` cycle | `while True:` heartbeat |
| **Sanitization** | Handle case & whitespace | `.lower().strip()` |
| **Knowledge Base** | Dictionary with 5+ intents | 30+ intents, multiple responses each |
| **Fallback** | Default for unknown inputs | `random.choice(fallbacks)` |
| **Exit Strategy** | Clean break command | `if clean in ("exit", "quit") → break` |

---

## ❌ Anti-Pattern vs ✅ Professional Approach

### The IF-ELIF Ladder — The Anti-Pattern
```python
# BAD: O(n) — scans every condition. Fragile. Hard to maintain.
if user_input == "hello":
    print("Hi!")
elif user_input == "bye":
    print("Goodbye!")
elif user_input == "what is ai":
    print("AI is...")
# ...50 more elif blocks = cascading failure risk
```

### Dictionary + `.get()` — The Professional Approach
```python
# GOOD: O(1) — instant lookup regardless of size.
responses = {
    "hello": "Hi there!",
    "bye":   "Goodbye!"
}
reply = responses.get(user_input, "I do not understand.")
```

> At 10,000 rules: the dictionary is **~100x faster** than the if-elif ladder.

---

## 🤖 DecoBot — Intent Categories

| Category | Examples |
|----------|---------|
| Greetings | hello, hi, hey, good morning, good evening |
| About DecoBot | who are you, what can you do, are you AI |
| AI Concepts | what is AI, machine learning, deep learning, KNN, NLP, overfitting |
| Python | what is Python, what is a dictionary, what is a loop |
| DecodeLabs | what is DecodeLabs, what is project 1, what is project 2 |
| Time & Date | what time is it, what is the date, what day is it |
| Small Talk | how are you, thank you, I am sad, I am fine |
| Fun | tell me a joke |
| Exit | exit, quit, bye, goodbye |

---

## 🚀 Getting Started

### Run the standalone script (Terminal)

```bash
git clone https://github.com/YOUR_USERNAME/rule-based-chatbot.git
cd rule-based-chatbot
python chatbot.py
```

### Run the notebook (Jupyter / Colab)

```bash
pip install notebook matplotlib
jupyter notebook rule_based_chatbot.ipynb
```

> **Alternative:** Upload to [Google Colab](https://colab.research.google.com) — zero setup needed.

---

## 💬 Sample Conversation

```
==============================================================
  🤖  DecoBot — Rule-Based AI Chatbot
  DecodeLabs | Project 1 | Batch 2026
==============================================================

DecoBot: Hello, Engineer! I am DecoBot — your deterministic AI assistant.

You: hello
DecoBot: Hi there! What can I do for you?

You: what is ai
DecoBot: Artificial Intelligence is the simulation of human intelligence
         in machines. It includes Rule-Based (deterministic) and Machine
         Learning (probabilistic) systems.

You: tell me a joke
DecoBot: Why do programmers prefer dark mode? Because light attracts bugs! 🐛😂

You: what is project 2
DecoBot: Project 2 is Data Classification Using AI. You build a KNN
         classifier on the Iris dataset using scikit-learn.

You: exit
DecoBot: Goodbye, Engineer! Keep building and keep learning. 👋
```

---

## 🔑 Key Concepts Learned

**Why Sanitization?** Users type inconsistently — `"HeLLo"`, `"  hello "`, `"HELLO"` should all trigger the same response. `.lower().strip()` normalizes all inputs to a clean format before matching.

**Why Dictionary over if-elif?** A Python dictionary is a hash map with O(1) constant-time lookup. An if-elif chain is O(n) — it scans every condition until a match is found. As your rule set grows, the dictionary stays instant while the ladder gets slower.

**Why `while True` with `break`?** A chatbot must keep running until the user decides to stop — not after a fixed number of turns. The infinite loop with a kill command (`exit`/`quit`) is the standard pattern for interactive CLI applications.

**The White Box Advantage:** Every response is 100% traceable — Input → Logic → Output. No mystery, no hallucination risk, 100% hard-coded. This is why rule-based systems are essential in finance and healthcare compliance.

---

## 🛠️ Technologies Used

| Tool | Purpose |
|------|---------|
| `Python 3.8+` | Core language |
| `random` | Response variety (multiple replies per intent) |
| `datetime` | Live time & date responses |
| `matplotlib` | Benchmarking chart (notebook only) |

---

## 🔮 What's Next (Project 2 Preview)

> *"From discrete key→value mapping... to continuous vector→class mapping."*

In Project 2, the rigid dictionary lookup is replaced by a **K-Nearest Neighbors classifier** that maps a 4-dimensional Iris flower measurement vector to one of 3 species classes — learning the mapping from data rather than hard-coding it.

---

## 👤 Author

**[Your Name]**  
AI Engineering Intern — DecodeLabs Batch 2026

---

## 🏢 About DecodeLabs

DecodeLabs is an industrial training organization based in Greater Lucknow, India, building real-world AI engineering skills through hands-on project-based learning.

📞 +91 89330 06408 | ✉️ decodelabs.tech@gmail.com | 🌐 [www.decodelabs.tech](http://www.decodelabs.tech)

---

*Project 1 of the DecodeLabs AI Industrial Training Kit — Batch 2026* 🛡️
