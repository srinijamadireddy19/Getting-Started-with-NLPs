# 🧠 Disaster Tweets Classification – Kaggle Competition

This repository contains my solution to the **[Natural Language Processing with Disaster Tweets](https://www.kaggle.com/competitions/nlp-getting-started)** Kaggle competition.  
The task is to build a model that can predict whether a given tweet is about a real disaster or not.

---

## 🚀 Project Overview

The goal of this project is to classify tweets as **real disaster-related** (`1`) or **not disaster-related** (`0`) using Natural Language Processing (NLP) and Machine Learning techniques.

The notebook in this repository demonstrates:
- Text preprocessing (cleaning, tokenization, stopword removal)
- Feature extraction using TF-IDF / Word Embeddings
- Model training and evaluation
- Submission file generation for Kaggle

---


---

## 🧩 Approach

1. **Data Cleaning & Preprocessing**
   - Removed URLs, mentions, hashtags, punctuation, and stopwords  
   - Tokenized text and normalized case  
   - Used lemmatization/stemming to reduce word forms

2. **Feature Engineering**
   - Used TF-IDF Vectorization / Word2Vec / BERT embeddings (depending on version)
   - Experimented with text length and keyword-based features

3. **Modeling**
   - Baseline: Logistic Regression  
   - Advanced: LSTM / BERT-based transformer model (used)  
   - Cross-validation for model robustness

4. **Evaluation**
   - Measured F1-score and accuracy on validation set  
   - Generated Kaggle submission in correct format

---

## 📊 Results

| Model | Validation F1 | Kaggle Score |
|--------|----------------|--------------|
| Logistic Regression | 0.81 | 0.80 |
| LSTM (Glove) | 0.51 | 0.82 |
| BERT (base uncased) | 0.85 | 0.84 |



---

## 🧠 Key Learnings

- Effective preprocessing drastically impacts performance.  
- Simpler models with TF-IDF often perform competitively with deep models.  
- Kaggle’s public LB can be misleading — always validate properly.

---

## 🛠️ Dependencies

To run locally:

```bash
pip install -r requirements.txt
