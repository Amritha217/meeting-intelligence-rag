# 🧠 Meeting Intelligence System (RAG + Timeline Memory)

## 🚀 Overview

A Retrieval-Augmented Generation (RAG) system that analyzes meeting transcripts and enables intelligent querying over decisions, action items, and discussions.

Users can ask:

* “What decisions were made last week?”
* “What tasks are pending?”
* “What was discussed about the API?”

---

## 🔥 Key Features

### ✅ Time-Aware Retrieval

* Filters answers based on time (e.g., last week)
* Enables temporal reasoning over meetings

### ✅ Structured Metadata Tagging

Each chunk is classified into:

* decision
* action_item
* discussion
* unresolved

---

### ✅ Hybrid Retrieval (IMPORTANT)

* Combines:

  * semantic search (embeddings)
  * keyword matching
* Improves precision significantly

---

### ✅ Multi-Meeting Memory

* Supports multiple meeting transcripts
* Query across meetings using `meeting_id`

---

### ✅ Retrieval Transparency

* Displays:

  * retrieved chunks
  * timestamps
  * metadata

---

### 📊 Timeline Visualization

* Visualizes decisions/tasks over time
* Helps identify trends across meetings

---

## 🧠 Architecture

User Query
↓
Query Understanding (intent + time)
↓
Metadata Filtering (tag + date)
↓
Hybrid Retrieval (semantic + keyword)
↓
LLM Generation (FLAN-T5)

---

## 🛠 Tech Stack

* **Language**: Python
* **LLM**: Hugging Face (FLAN-T5)
* **Embeddings**: sentence-transformers
* **Vector DB**: ChromaDB
* **Framework**: LangChain
* **UI**: Streamlit

---

## ▶️ How to Run

```bash
pip install -r requirements.txt
streamlit run app.py
```

---

## 💡 Example Queries

* What decisions were made last week?
* What tasks are assigned?
* What discussions happened about the API?

---

## 🎯 Why This Project Stands Out

* Goes beyond basic RAG
* Implements **time-aware retrieval**
* Uses **structured metadata**
* Combines **semantic + keyword search**
* Shows **retrieval transparency**

---

## 🚀 Future Improvements

* LLM-based query understanding
* Persistent database (PostgreSQL)
* Multi-user support
* Deployment (Streamlit Cloud / AWS)

---

## 👨‍💻 Author

Your Name
