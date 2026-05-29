# Mini RAG Chatbot using FAISS

A Retrieval-Augmented Generation (RAG) chatbot built using Python, FAISS, Sentence Transformers, and Hugging Face models. This project enables users to upload a PDF document and ask questions about its contents using semantic search and Large Language Models (LLMs).

---

## Project Overview

This project implements a complete RAG pipeline from scratch:

1. PDF Text Extraction
2. Text Chunking
3. Embedding Generation
4. Vector Storage using FAISS
5. Semantic Search
6. Context Retrieval
7. LLM-based Answer Generation

The chatbot retrieves the most relevant sections from a PDF and uses them as context to generate accurate answers.

---

## Features

* Extract text from PDF documents
* Split large documents into manageable chunks
* Generate semantic embeddings using Sentence Transformers
* Store embeddings in FAISS vector database
* Perform similarity search on user queries
* Retrieve top relevant chunks
* Generate context-aware answers using an LLM
* Interactive chatbot interface

---

## Tech Stack

| Component            | Technology                      |
| -------------------- | ------------------------------- |
| Language             | Python                          |
| Notebook             | Jupyter Notebook / Google Colab |
| PDF Processing       | PyPDF                           |
| Embeddings           | Sentence Transformers           |
| Vector Database      | FAISS                           |
| LLM                  | FLAN-T5                         |
| Numerical Operations | NumPy                           |

---

## Architecture

```text
PDF
 ↓
Text Extraction
 ↓
Chunking
 ↓
Embeddings Generation
 ↓
FAISS Vector Database
 ↓
Semantic Search
 ↓
Relevant Context Retrieval
 ↓
Prompt Construction
 ↓
LLM
 ↓
Final Answer
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/mini-rag-chatbot.git

cd mini-rag-chatbot
```

Install dependencies:

```bash
pip install faiss-cpu
pip install sentence-transformers
pip install transformers
pip install torch
pip install pypdf
```

---

## Usage

### 1. Add Your PDF

Place your PDF file in the project directory.

Example:

```python
PDF_PATH = "Cybersecurity.pdf"
```

### 2. Run the Notebook

Open:

```text
Mini_RAG_Chatbot.ipynb
```

Run all cells sequentially.

### 3. Ask Questions

Example:

```python
question = "What is malware and explain its types?"
```

Output:

```text
Malware is malicious software designed to damage, disrupt,
or gain unauthorized access to computer systems.

Types of malware include:
• Virus
• Worm
• Trojan Horse
• Spyware
• Ransomware
• Adware
```

---

## Example Questions

### Cybersecurity PDF

* What is malware?
* Explain ransomware.
* What is phishing?
* What is a firewall?
* Difference between virus and worm?

### Artificial Intelligence PDF

* What is machine learning?
* Explain supervised learning.
* What is deep learning?
* What is overfitting?

### DBMS PDF

* What is normalization?
* Explain ACID properties.
* What is a primary key?
* What is indexing?

---

## Project Structure

```text
Mini-RAG-Chatbot/
│
├── Mini_RAG_Chatbot.ipynb
├── sample.pdf
├── README.md
└── requirements.txt
```

---

## Learning Outcomes

This project demonstrates:

* Retrieval-Augmented Generation (RAG)
* Semantic Search
* Embedding Models
* Vector Databases
* Prompt Engineering
* Context-Aware Question Answering
* Large Language Models

---

## Future Improvements

* Streamlit Web Interface
* Conversational Memory
* Support for Multiple PDFs
* Hybrid Search (Keyword + Semantic)
* ChromaDB/Pinecone Integration
* OpenAI GPT Integration
* Source Citation Support

---

## Results

The chatbot successfully retrieves relevant document chunks using FAISS and generates answers grounded in the provided PDF context, reducing hallucinations and improving response accuracy.

---

## Author

Developed as a Mini RAG Chatbot project for learning Retrieval-Augmented Generation, Vector Databases, and LLM-powered Question Answering.
