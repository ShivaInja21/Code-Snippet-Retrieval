# 🧠 Code Snippet Retrieval System

## 📌 Overview

This project implements a **Code Snippet Retrieval System** that retrieves relevant code snippets based on a **natural language query**. The system uses **classical Information Retrieval (IR) techniques** to match user queries with code snippets by measuring textual similarity.

The project demonstrates how **TF-IDF vectorization** and **cosine similarity** can be used to build a simple yet effective semantic search system for code.

---

## 🎯 Problem Statement

Developers often know *what they want to do* but find it difficult to locate the right code implementation quickly. Traditional keyword-based searches are limited and fail to capture semantic meaning.

This project addresses the problem by:
- Treating code snippets as searchable documents
- Ranking them based on relevance to a user’s query

---

## 🧠 Approach

The system follows a **Vector Space Model (VSM)**–based retrieval pipeline:

### 1. Dataset Preparation
- A dataset of Python code snippets with corresponding natural-language descriptions
- The dataset was **manually created using web scraping**
- Only the **final curated dataset** is included in this repository
- Dataset creation (scraping) code is **not included** in this project

### 2. Text Preprocessing
- Lowercasing
- Tokenization
- Stop-word removal
- Stemming using:
  - Porter Stemmer
  - Snowball Stemmer

### 3. Feature Extraction
- TF-IDF (Term Frequency–Inverse Document Frequency) vectorization

### 4. Similarity Matching
- Cosine similarity between query vectors and code snippet vectors

### 5. Retrieval
- Returns the **top-K most relevant code snippets** ranked by similarity score

---

## 🧩 Model Used

- **TF-IDF Vector Space Model**
- **Cosine Similarity**

📌 This project does **not** use deep learning, transformer models, or embeddings.  
It focuses on **classical statistical Information Retrieval techniques**.

---

## 📊 Evaluation

- This is a **retrieval system**, not a classification model
- No labeled ground-truth dataset is available
- Therefore, traditional accuracy metrics (accuracy, precision, recall, F1-score) are **not computed**

Retrieval quality is evaluated **qualitatively** by inspecting ranked outputs for different queries.

---

## 🛠️ Technologies Used

- **Python**
- **NLTK**
- **Scikit-learn**
- **NumPy**
- **Jupyter Notebook**
