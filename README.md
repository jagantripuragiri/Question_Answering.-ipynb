# 📄 Document-based Question Answering System using Docling & Granite 3.1

## 🚀 Overview
This project demonstrates how to build a **document-based question answering system** using **Docling** for document parsing and the **IBM Granite 3.1 (8B-Instruct)** model for large language understanding.

The system extracts text from various document formats, embeds the content, and uses **Retrieval-Augmented Generation (RAG)** to provide accurate, context-aware answers to user queries.

---

## 🧠 What is Docling?

**Docling** is an open-source document processing toolkit by **IBM** that enables parsing and exporting of various document formats into structured data formats like Markdown or JSON.  

### 🔹 Supported Input Formats
- PDF  
- DOCX  
- PPTX  
- XLSX  
- Images  
- HTML  
- AsciiDoc  
- Markdown  

### 🔹 Key Features
- Converts documents into structured formats (Markdown/JSON)  
- Supports **OCR (Optical Character Recognition)** for scanned documents  
- Ideal for use cases like:
  - Medical record digitization  
  - Banking document extraction  
  - Travel document verification  

---

## ⚙️ Retrieval-Augmented Generation (RAG) and Large Context Windows

**Retrieval-Augmented Generation (RAG)** is an architecture that connects **Large Language Models (LLMs)** with external knowledge bases — without the need for fine-tuning or retraining.  

### 🔸 How RAG Works
1. Extract and embed text from documents  
2. Store embeddings in a vector database (e.g., FAISS, Chroma)  
3. Retrieve relevant chunks when a user asks a question  
4. Provide the retrieved context to the LLM for accurate, grounded responses  

This approach enhances **accuracy, factual consistency**, and **context relevance** in generative AI outputs.

---

## 🧩 Granite 3.1 Model

The **IBM Granite-3.1-8B-Instruct** model is a powerful open-source LLM optimized for instruction-based tasks.  
It supports a **context window of up to 128K tokens**, allowing the model to process large amounts of information in a single query.  

In this project:
- The model is accessed **locally using [Ollama](https://ollama.ai/)** (no API key required)
- It can also be accessed via **[Hugging Face](https://huggingface.co/)**

---

## 🧠 Architecture Workflow

1. Parse document content using **Docling**
2. Split text into smaller **chunks**
3. Generate embeddings and store them in a **vector database**
4. Retrieve top relevant chunks using **semantic similarity**
5. Feed retrieved context to **Granite 3.1** for answer generation



---

## 🔗 Reference
IBM Official Tutorial:  
👉 [Build a Document Question Answering System with Docling and Granite 3.1](https://www.ibm.com/think/tutorials/build-document-question-answering-system-with-docling-and-granite?utm_medium=OSocial&utm_source=Youtube&utm_content=WAIWW&utm_id=YT-Applied-AI-Document-Question-Answering-with-Granite)

---

## 🧰 Tech Stack
- **Python**
- **Docling**
- **Granite 3.1 LLM**
- **LangChain**
- **Ollama**
- **FAISS / Chroma**
- **Hugging Face Transformers**

---

## 🧪 Future Enhancements
- Integrate a **web-based UI** for document upload and query  
- Add **multi-document support**  
- Deploy using **AWS Lambda / Azure Functions**  
- Implement **user authentication and session history**

---

### 🏁 Author
**Jagan Tripuragiri**  
AI Developer | Machine Learning Enthusiast  
📫 [LinkedIn](https://www.linkedin.com/in/jagantripuragiri/) | 💻 [GitHub](https://github.com/jagantripuragiri)
