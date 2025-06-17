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

## 🏗️ Architecture

```mermaid
graph TD
  A[PDF Upload via Colab] --> B[PyPDFLoader (LangChain)]
  B --> C[Text Splitter (Recursive Chunking)]
  C --> D[Nomic-Embed Embeddings (Ollama)]
  D --> E[ChromaDB Vector Store]
  E --> F[Retriever with MMR Search]
  F --> G[DeepSeek-R1 LLM (Ollama)]
  G --> H[Final Answer + Source Documents]
