# 🧠 DocuSense: Retrieval-Augmented PDF QA System  
![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)  
![LangChain](https://img.shields.io/badge/LangChain-RAG-yellow?logo=readthedocs)  
![LLM](https://img.shields.io/badge/DeepSeek-LLM-orange?logo=OpenAI)  
![Status](https://img.shields.io/badge/Project-Type-Research%20%7C%20Resume%20Ready-brightgreen)  

> An intelligent RAG-based system that lets you query uploaded PDFs using powerful language models and custom embeddings.

---

## 🚀 Overview

**DocuSense** is a Retrieval-Augmented Generation (RAG) pipeline that allows users to query their own documents in natural language. It combines LangChain, DeepSeek (via Ollama), Nomic-Embed, and ChromaDB for full PDF-to-answer functionality.

---

### 🏗️ Stack

- **LangChain** for chaining, retrieval & orchestration  
- **DeepSeek-R1 (via Ollama)** for LLM-based responses  
- **Nomic-Embed Text** for generating custom vector embeddings  
- **ChromaDB** as the vector store  
- **PyPDF + Recursive Splitter** for parsing & chunking  
- **Python + Colab** for implementation and testing

---

## 📂 Features

✅ Upload one or more PDFs  
✅ Process & chunk documents with context overlap  
✅ Embed using Nomic (Ollama) or OpenAI  
✅ Smart retrieval using **MMR Search**  
✅ Ask context-aware questions with accurate source tracing  
✅ Clean code, modular structure — ready for demos and research

---

## 🏗️ Architecture

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

