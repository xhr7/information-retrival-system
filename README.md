# 🧠 Information Retrieval System

[![Demo](https://github.com/xhr7/information-retrival-system/assets/102740867/6dd6875c-1116-42b5-b07c-6942e2618a75)](https://github.com/xhr7/information-retrival-system/assets/102740867/6dd6875c-1116-42b5-b07c-6942e2618a75
)

[![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python)](https://www.python.org/)
[![NLTK](https://img.shields.io/badge/NLTK-NLP-green?style=for-the-badge)](https://www.nltk.org/)
[![TF-IDF](https://img.shields.io/badge/TF--IDF-TermWeighting-orange?style=for-the-badge)]()
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-yellow?style=for-the-badge&logo=scikitlearn)](https://scikit-learn.org/)
[![Flask](https://img.shields.io/badge/Flask-UsedForUI-black?style=for-the-badge&logo=flask)]()
[![Google Colab](https://img.shields.io/badge/Colab-EasyRun-orange?style=for-the-badge&logo=googlecolab)]()

---

## 🌐 Overview

This is a mini search engine that simulates how Information Retrieval (IR) systems work.  
The system can:
- Index `.txt` documents
- Process user queries
- Rank documents by relevance using **TF-IDF** and **cosine similarity**
- Display results using a simple **Flask-based web interface**


## 📦 Features

| Feature                       | Description                                                                 |
|------------------------------|-----------------------------------------------------------------------------|
| Tokenization & Preprocessing | Handles punctuation, lowercasing, and stopwords removal                    |
| Stemming & Lemmatization     | Combines both techniques for better word normalization                     |
| TF-IDF Term Weighting        | Assigns importance scores to terms based on frequency & uniqueness         |
| Query Vectorization          | Transforms user input into a vector using the same preprocessing pipeline  |
| Cosine Similarity Scoring    | Measures similarity between query and documents                            |
| Flask Web Interface          | Simple web UI for entering queries and viewing ranked results              |
| Ranked File Output           | Displays documents sorted by relevance to the user's query                 |


---

## 🗂️ Project Structure

```bash
📁 doc/
│   ├── birds.txt               # Unrelated topic
│   ├── saffron.txt             # Unrelated topic
│   ├── stack.txt               # Related to data structures
│   ├── queue.txt
│   ├── ...
│
📁 doc_clear/                   # Cleaned documents after preprocessing
│   ├── stack.txt
│   ├── queue.txt
│   └── ...
│
📄 project_final.ipynb          # Final implementation notebook with all logic
📄 app.py                       # Flask code for running the user interface
```




## 🧪 How It Works (Workflow)

1. **Document Collection**
   - 12 `.txt` files created: 10 about data structures, 2 on unrelated topics ("birds", "saffron")

2. **Preprocessing**
   - Tokenization
   - Lowercasing
   - Stopword removal using `nltk`
   - Punctuation & special character removal
   - Stemming + Lemmatization for better normalization

3. **Indexing**
   - Vector representation using **TF-IDF**
   - Weighting each word based on its importance in the document

4. **Query Handling**
   - User inputs query
   - Query processed using same steps as documents

5. **Ranking**
   - Calculate cosine similarity between query vector and each document
   - Return top relevant files (ranked descending)
  
## 🚀 Getting Started

### 🔧 Prerequisites

- Python 3.10+
- Google Colab (recommended)
- Basic knowledge of NLP concepts

### ⚙️ Installation

```bash
git clone https://github.com/xhr7/information-retrival-system.git
cd information-retrival-system
