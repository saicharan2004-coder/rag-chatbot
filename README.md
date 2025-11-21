# 📚 Simple RAG Chatbot (Python)

A lightweight **Retrieval-Augmented Generation (RAG)** chatbot built using:

* **SentenceTransformers** → text embeddings
* **FAISS** → vector search
* **Python** → simple console interface

This project is intentionally minimal and production-ready so you can quickly showcase your skills to companies or add it to your portfolio.

---

## 🚀 Features

* Loads documents from the `docs/` folder
* Converts documents into embeddings
* Stores embeddings in a FAISS index
* Retrieves the most relevant document for any user query
* Clean and minimal Python script

---

## 📁 Project Structure

```
simple-rag-chatbot/
│
├── main.py
├── requirements.txt
├── README.md
└── docs/
     └── sample.txt
```

---

## 🛠️ Installation

### 1️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 2️⃣ Add your documents

Place any `.txt` files inside the `docs/` folder.
Example:

```
docs/
 ├── finance_notes.txt
 ├── faq.txt
 └── product_info.txt
```

---

## ▶️ Running the Chatbot

```bash
python main.py
```

You will see:

```
Simple RAG Chatbot Ready!
You:
```

Type your question and the bot will retrieve the most relevant document.

Example:

```
You: what is in the sample doc?

AI Retrieved Document:
This is a sample document for the RAG chatbot. Add more files in /docs.
```

Type `exit` or `quit` to stop the chatbot.

---

## 📌 How It Works (Quick Overview)

1. Loads `.txt` files
2. Generates embeddings using **MiniLM-L6-v2**
3. FAISS stores vectors for fast similarity search
4. User query → converted to embedding
5. Nearest document is returned

This is a foundational RAG model similar to what many AI companies build.

---

## 📦 Dependencies

```
faiss-cpu  
sentence-transformers  
numpy
```

---

## ⭐ Use Cases

* FAQ retrieval
* Document-based answering
* Chatbots for small knowledge bases
* Portfolio demonstration
* AI/ML learning projects

---

## 🤝 Contribution

Feel free to fork, improve, and submit pull requests!

---

## 📜 License

MIT License

