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

---

## 📦 Features

- Tokenization & preprocessing (stopwords, casing, punctuation)
- Stemming & lemmatization (combined for better normalization)
- TF-IDF term weighting
- Query vectorization
- Cosine similarity scoring
- Web interface with Flask
- Returns ranked list of relevant files

---

## 🧰 Technologies Used

- ![Python](https://img.shields.io/badge/-Python-informational?style=flat&logo=python&logoColor=white&color=3670A0)
- ![NLTK](https://img.shields.io/badge/-NLTK-green?style=flat&logo=nltk&logoColor=white)
- ![Scikit-learn](https://img.shields.io/badge/-Scikit--learn-orange?style=flat&logo=scikit-learn&logoColor=white)
- ![Flask](https://img.shields.io/badge/-Flask-black?style=flat&logo=flask&logoColor=white)
- ![Google Colab](https://img.shields.io/badge/-Google_Colab-yellow?style=flat&logo=googlecolab&logoColor=white)

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
