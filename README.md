<div align="center">

# 🇮🇷 Persian RAG with LangChain

**Question answering over Persian text using multilingual embeddings, vector stores and a local LLM.**

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?logo=langchain&logoColor=white)
![Hugging Face](https://img.shields.io/badge/🤗_Hugging_Face-FFD21E)
![FAISS](https://img.shields.io/badge/FAISS-0467DF)
![Colab](https://img.shields.io/badge/Open_in-Colab-F9AB00?logo=googlecolab&logoColor=white)

</div>

---

## ✨ Overview

`huggingface.ipynb` builds a retrieval-augmented question-answering system for the **Persian** language:

1. 📚 Loads the **PQuAD** Persian QA dataset (`alienit/PQuAD`) with Hugging Face `datasets` and converts it to documents (`CSVLoader`).
2. ✂️ Splits the text into chunks with `RecursiveCharacterTextSplitter`.
3. 🧬 Embeds the chunks with the multilingual **`BAAI/bge-m3`** model.
4. 🗄️ Stores vectors in **FAISS** and in a persistent **ChromaDB** collection.
5. 💬 Answers questions with a `ConversationalRetrievalChain` that keeps conversation memory.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Arashomranpour/persian_LLM/blob/main/huggingface.ipynb)

## 🚀 Getting Started

```bash
git clone https://github.com/Arashomranpour/persian_LLM.git
cd persian_LLM
pip install langchain datasets sentence-transformers faiss-cpu chromadb pandas jupyter
jupyter notebook huggingface.ipynb
```

## 📁 Project Structure

```
.
├── huggingface.ipynb   # Dataset, embeddings, vector stores, QA chain
└── test.txt            # Sample text for testing
```

## 🛠️ Tech Stack

`LangChain` · `Hugging Face (datasets, BGE-M3)` · `FAISS` · `ChromaDB`
