LLM Hallucination Detector

Research Project by Sneha Kumari J
B.Tech Artificial Intelligence & Machine Learning | Presidency University, Bengaluru

---

 Overview
An intelligent system that automatically detects hallucinations 
in Large Language Model responses by comparing outputs against 
a ground truth knowledge base using semantic similarity scoring.

---

 System Architecture
Question → LLM Response Generation
                    ↓
Ground Truth Knowledge Base
                    ↓
Semantic Similarity Scoring (Sentence Transformers)
                    ↓
Hallucination Risk Classification
                    ↓
Visual Analysis Dashboard

---

 Modules

 Module 1 — Knowledge Base
- Ground truth fact storage
- Covers AI, science, geography domains
- Extensible to any domain

Module 2 — LLM Response Generator
- LLaMA 3.1 via Groq API
- Tests both real and fake questions
- Low temperature for consistent responses

Module 3 — Hallucination Scoring Engine
- Sentence Transformer embeddings
- Cosine similarity measurement
- Three tier risk classification
- Handles unknown questions

Module 4 — Visualization Dashboard
- Hallucination scores per question
- Risk level distribution
- Semantic similarity analysis

---

Risk Classification

| Score | Risk Level | Verdict |
|---|---|---|
| 0.0 - 0.3 | Low | Factual ✅ |
| 0.3 - 0.6 | Medium | Uncertain ⚠️ |
| 0.6 - 1.0 | High | Hallucination 🚨 |

---

Tech Stack
- Python
- Groq API + LLaMA 3.1 8B
- Sentence Transformers
- Cosine Similarity
- Pandas, NumPy
- Matplotlib, Seaborn

---

Key Findings
1. LLMs confidently hallucinate about non existent people and events
2. Semantic similarity effectively identifies factual inconsistencies
3. Questions without ground truth show highest hallucination risk
4. Uncertainty phrases indicate self aware LLM behavior

---

 Research Relevance
- AI Safety and Reliability
- LLM Evaluation Frameworks
- Trustworthy AI Systems
- Fact Verification
- Responsible AI Development

---

 Connection To Previous Research
This project is a natural extension of:
- LLM Behavior & Prompt Engineering Study
- RAG Document QA System

Together they form a complete LLM research pipeline:
Study Behavior → Detect Failures → Ground With RAG

---

Author
Sneha Kumari J
- LinkedIn: https://www.linkedin.com/in/sneha-kumari-computer-engineering
- Email: snehakumari1869@gmail.com
