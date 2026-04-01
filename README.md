# 🧠 Meeting Intelligence System (RAG + Timeline Memory)

## 🚀 Overview

A Retrieval-Augmented Generation (RAG) system that analyzes meeting transcripts .

Users can ask:

* “What decisions were made last week?”
* “What tasks are pending?”
* “What was discussed about the API?”

---

## 🔥 Key Feature

### ✅ Time-Aware Retrieval

* Filters answers based on time (e.g., last week)
* Enables temporal reasoning over meetings


---

### ✅  Retrieval 

* semantic search (embeddings)
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
Metadata Filtering (date)
↓
Retrieval (semantic )
↓
LLM Generation (FLAN-T5)

---

## 🛠 Tech Stack

* **Language**: Python
* **LLM**: Hugging Face (FLAN-T5)
* **Embeddings**: sentence-transformers
* **Vector DB**: ChromaDB
* **Framework**: LangChain


---



## 💡 Example Queries

* What decisions were made last week?
* What tasks are assigned?
* What discussions happened about the API?


---

## 👨‍💻 Author

Amritha Dileep Kumar
