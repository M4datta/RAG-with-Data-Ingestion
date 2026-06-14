# 📚 RAG with Data Ingestion using LangChain

A comprehensive hands-on project demonstrating how to ingest, parse, and prepare data from multiple sources for Retrieval-Augmented Generation (RAG) applications using LangChain.

This repository covers document loading, metadata extraction, text splitting, and structured/unstructured data processing from various file formats commonly used in enterprise AI systems.

---

## 🚀 Project Overview

Retrieval-Augmented Generation (RAG) systems are only as good as the data they can retrieve.

This project focuses on the **Data Ingestion Layer** of a RAG pipeline by demonstrating how to:

* Load and process documents
* Extract metadata
* Parse PDFs and Word documents
* Read CSV and Excel files
* Process JSON and JSONL datasets
* Extract information from SQL databases
* Prepare documents for chunking and embedding

The project is ideal for anyone learning:

* LangChain
* RAG Architecture
* Document Processing
* Vector Databases
* Enterprise AI Applications
* Data Engineering for LLMs

---

## 🏗️ RAG Architecture

The ingestion layer is the first step in a modern RAG system:

```text
Data Sources
      │
      ▼
Document Loaders
      │
      ▼
Text Extraction
      │
      ▼
Chunking & Splitting
      │
      ▼
Embeddings
      │
      ▼
Vector Database
      │
      ▼
Retriever
      │
      ▼
LLM Response
```

---

## 📂 Project Structure

```text
RAG-with-Data-Ingestion/
│
├── 1-dataingestion.ipynb
├── 2-dataparsingpdf.ipynb
├── 3-dataparsingdoc.ipynb
├── 4-csvexcelparsing.ipynb
├── 5-jsonparsing.ipynb
├── 6-databaseparsing.ipynb
│
├── attention.pdf
├── proposal.docx
├── proposal.txt
├── python_intro.txt
│
├── products.csv
├── inventory.xlsx
│
├── company_data.json
├── events.jsonl
│
├── company.db
│
├── rag-architecture-diagram.svg
└── README.md
```

---

## 📖 Notebook Breakdown

### 1️⃣ Data Ingestion Fundamentals

**File:** `1-dataingestion.ipynb`

Topics Covered:

* LangChain Document objects
* Metadata management
* Document structure
* Text splitting techniques

Loaders and Splitters:

* Document
* RecursiveCharacterTextSplitter
* CharacterTextSplitter
* TokenTextSplitter

Key Learning:

Understand how LangChain represents documents before indexing them into vector databases.

---

### 2️⃣ PDF Parsing

**File:** `2-dataparsingpdf.ipynb`

Topics Covered:

* PDF document loading
* Metadata extraction
* Page-level document processing

Loaders:

* PyPDFLoader
* PyMuPDFLoader

Key Learning:

Extract and prepare content from PDF files for embedding and retrieval.

---

### 3️⃣ Word Document Parsing

**File:** `3-dataparsingdoc.ipynb`

Topics Covered:

* DOCX processing
* Structured content extraction
* Metadata handling

Loaders:

* Docx2txtLoader
* UnstructuredWordDocumentLoader

Key Learning:

Convert Word documents into searchable LangChain documents.

---

### 4️⃣ CSV & Excel Parsing

**File:** `4-csvexcelparsing.ipynb`

Topics Covered:

* Reading tabular data
* Product inventory datasets
* Converting structured data into documents

Technologies:

* Pandas
* CSV Files
* Excel Files

Key Learning:

Prepare business datasets for retrieval and question answering.

---

### 5️⃣ JSON Parsing

**File:** `5-jsonparsing.ipynb`

Topics Covered:

* Nested JSON structures
* JSONL processing
* Complex data extraction

Technologies:

* JSON
* JSON Lines (JSONL)

Key Learning:

Transform hierarchical JSON data into retrieval-ready documents.

---

### 6️⃣ Database Parsing

**File:** `6-databaseparsing.ipynb`

Topics Covered:

* SQLite integration
* Database querying
* Structured data ingestion

Database:

* SQLite (`company.db`)

Key Learning:

Connect enterprise databases to RAG pipelines.

---

## 🛠️ Technologies Used

* Python
* LangChain
* Pandas
* SQLite
* PyPDF
* PyMuPDF
* Docx2txt
* Unstructured
* Jupyter Notebook

---

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/RAG-with-Data-Ingestion.git

cd RAG-with-Data-Ingestion
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate:

### Windows

```bash
.venv\Scripts\activate
```

### Linux / Mac

```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install langchain
pip install langchain-community
pip install pandas
pip install pypdf
pip install pymupdf
pip install docx2txt
pip install unstructured
pip install openpyxl
```

Or:

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Run notebooks in order:

```text
1-dataingestion.ipynb
↓
2-dataparsingpdf.ipynb
↓
3-dataparsingdoc.ipynb
↓
4-csvexcelparsing.ipynb
↓
5-jsonparsing.ipynb
↓
6-databaseparsing.ipynb
```

---

## 🎯 Learning Outcomes

By completing this project, you will learn:

✅ LangChain Document Objects

✅ Metadata Management

✅ Text Chunking Strategies

✅ PDF Processing

✅ Word Document Processing

✅ CSV & Excel Data Parsing

✅ JSON & JSONL Processing

✅ Database Integration

✅ Data Preparation for Vector Databases

✅ Foundations of Enterprise RAG Systems

---

## 🔮 Future Enhancements

Potential next steps:

* Add OpenAI Embeddings
* Integrate FAISS
* Integrate ChromaDB
* Build a complete RAG chatbot
* Add LangGraph workflow
* Add Hybrid Search
* Deploy using Streamlit

---

## 👨‍💻 Author

This project was created to demonstrate practical data ingestion techniques required for modern Retrieval-Augmented Generation (RAG) systems using LangChain.

If you found this project helpful, consider giving it a ⭐ on GitHub.

---

## 📄 License

This project is licensed under the MIT License.
