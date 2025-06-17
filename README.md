# 🧠 DocuSense: Retrieval-Augmented PDF QA System  
![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)  
![LangChain](https://img.shields.io/badge/LangChain-RAG-yellow?logo=readthedocs)  
![LLM](https://img.shields.io/badge/DeepSeek-LLM-orange?logo=OpenAI)  
![Status](https://img.shields.io/badge/Project-Type-Research%20%7C%20Resume%20Ready-brightgreen)  

> A PDF Question Answering system using Retrieval-Augmented Generation (RAG) with LangChain, Ollama LLMs, and ChromaDB.

---

## 🚀 Overview

**DocuSense** is a smart PDF assistant built using LangChain, DeepSeek-R1 LLM (via Ollama), and ChromaDB. It leverages vector embeddings to retrieve and synthesize contextually relevant answers from uploaded documents in real-time.

---

## 🧰 Tech Stack

- **Python 3.10**
- **LangChain** (RetrievalQA + document loaders)
- **Ollama** with **DeepSeek-R1** for LLM inference
- **Nomic-Embed Text** for generating vector embeddings
- **ChromaDB** for semantic vector storage and fast retrieval
- **Google Colab** for notebook-based interactivity

---



## 🏗️ DocuSense Architecture

The following diagram illustrates the internal workflow of the DocuSense RAG system — from PDF ingestion to LLM-driven QA output:

![DocuSense Architecture](mermaid-diagram-2025-06-18-011446.png)

