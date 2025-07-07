# 🤖 Loan Approval Q&A Chatbot using RAG and LLMs

An intelligent chatbot that answers questions about loan approvals using **Retrieval-Augmented Generation (RAG)** and a lightweight **Language Model (LLM)**.

> 🔍 Built with FAISS + Sentence Transformers + HuggingFace's `flan-t5-base`.  
> 🚀 Executes entirely in **Google Colab**, no paid API or login required.

---

## 📌 Project Overview

This project uses a **Loan Approval Dataset** to build a Q&A system where:

- User types a natural language question
- The system retrieves relevant rows from the dataset using **FAISS vector search**
- A **pretrained LLM** (flan-t5-base) generates a smart answer from those rows

---

## 🧠 Technologies Used

| Component              | Tool/Library                     |
|------------------------|----------------------------------|
| Dataset                | [Kaggle: Loan Approval Dataset](https://www.kaggle.com/datasets/sonalisingh1411/loan-approval-prediction) |
| Embedding Model        | `all-MiniLM-L6-v2` (Sentence-BERT) |
| Retriever              | `FAISS` (Facebook AI Similarity Search) |
| Language Model (LLM)   | `google/flan-t5-base` (HuggingFace) |
| Platform               | Google Colab                     |
| Programming Language   | Python                           |

---

## 🔧 How It Works

1. 📁 Upload `Training Dataset.csv`
2. 🧩 Each row is converted to a natural-language-like document
3. 🔍 FAISS retrieves the top matching rows for your query
4. 🤖 `flan-t5-base` generates a human-like answer using the retrieved context

---

## 🧪 Example Questions

- **"What is the most common loan status?"**
- **"How does credit history affect loan approval?"**
- **"What is the average applicant income?"**
- **"Are married applicants more likely to be approved?"**
- **"Which property areas have the highest approval rate?"**

---

## ✅ Features

- ❌ No fine-tuning required
- ✅ Lightweight & runs on free Colab GPU/CPU
- ✅ Doesn't need OpenAI keys or HuggingFace login
- ✅ Easily extendable to any tabular dataset
- 📚 Good example of combining classic ML tools (FAISS) with LLMs

---

## 📂 Folder Structure (Suggested)

```bash
loan-rag-chatbot/
├── rag_chatbot_colab.ipynb    # Google Colab notebook
├── training_dataset.csv       # Dataset from Kaggle (optional upload)
├── screenshots/               # Q&A proof images
└── README.md                  # This file
  # rag-loan-chatbot
