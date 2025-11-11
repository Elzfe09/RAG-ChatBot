# 🧭 MSIG Travel Insurance Chatbot – RAG + LangGraph + Agentic Tools

> “Empower your customers with instant, precise, and human-like responses about your insurance products — powered by your own private knowledge.”

---

## 💡 Project Overview
Everyone is now familiar with interactive AI chats such as **ChatGPT**, **Gemini**, and others — tools that generate answers from vast internet-scale knowledge (LLMs).  
But what if you want to build your **own AI question-answering system** based on **your organization’s private documents**?

This project demonstrates how to build a **Retrieval-Augmented Generation (RAG)** chatbot for **MSIG Travel Insurance**, where the system answers user questions based on the company’s **internal policy PDFs** — not public internet data.

---

## 🎯 Objective
Create an intelligent chatbot that can accurately respond to:  
- 🧳 Travel insurance inquiries  
- 💬 Customer doubts and clarifications  
- 📑 Policy coverage and differences  
- 💡 Product recommendations  

...without users having to manually search through long documents.

---

## ⚙️ Methodology

### 🔹 RAG (Retrieval-Augmented Generation)
1. **Document Loading** – Import PDF policy files  
2. **Chunking & Embedding** – Tokenize text and convert into numerical embeddings  
3. **Vector Storage** – Store semantic vectors in a vector database  
4. **Semantic Retrieval** – Match user questions to related document segments  
5. **LLM Integration** – Combine retrieved context with an LLM for natural responses

### 🔹 LangGraph Integration
Using **LangGraph**, the chatbot pipeline is modularized into:
- **State** – Stores conversation memory and retrieved info  
- **Nodes** – Define functional units like embedding, retrieval, or response generation  
- **Edges** – Control logic between nodes  
- **Graph** – Represents the full flow of reasoning

This structure makes the system **more flexible, debuggable, and expandable** compared to traditional sequential RAG pipelines.

---

## 🧠 Agentic Tooling
In addition to RAG, an **agentic retriever tool** is implemented using `create_retriever_tool()`.  
This allows the chatbot to dynamically invoke retrieval actions (e.g., searching policy content) **without hard-coded function calls**, creating a more **autonomous and adaptive** interaction loop.

---

## 💬 Expected Outcome
By the end of the project, users will experience a chatbot that:  
- Greets them naturally 👋  
- Recognizes their name and intent 🧍‍♂️  
- Provides accurate, context-aware answers 📚  
- Delivers smooth and friendly conversation 💫

Ultimately, this enhances **customer satisfaction** and helps users **understand travel insurance plans** before purchase — in a joyful and effortless way.

---

## 🚀 Tech Stack
- 🐍 **Python**  
- 🧩 **LangChain / LangGraph**  
- 📄 **PDF Data Loader (PyPDFLoader / Unstructured)**  
- 📊 **Vector Store (Chroma / FAISS)**  
- 🤖 **LLM (OpenAI, Groq, or Gemini API)**  
- 🧠 **Agentic Tools Framework**
