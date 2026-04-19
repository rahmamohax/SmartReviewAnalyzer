# 🧠 Smart Review Analyzer (NLP Project)

A complete Natural Language Processing pipeline for sentiment analysis and insight extraction from user reviews.  
This project classifies reviews into **positive / negative sentiment** and extracts **interpretable insights such as keywords, patterns, and explanations**.

---

## 🚀 Project Overview

This system is designed to go beyond simple sentiment classification.  
It not only predicts whether a review is positive or negative but also explains **why** using extracted insights.

### 🎯 Key Features:
- Full NLP preprocessing pipeline
- TF-IDF and Embedding-based feature extraction
- Baseline ML model (Logistic Regression / Naive Bayes)
- Deep learning model (LSTM or Transformer-based)
- Insight extraction (keywords, patterns, explanations)
- Model comparison and evaluation

---

## 📊 Problem Statement

Given a user review, the system should:

1. Classify sentiment (Positive / Negative)
2. Extract important keywords influencing prediction
3. Identify common patterns in reviews
4. Provide explanation for predictions

---

## 📁 Dataset

We use a labeled sentiment dataset (binary classification):
- Yelp / Amazon / IMDb reviews dataset (or combined dataset)

### Label Mapping:
- Positive → 1 (4–5 stars)
- Negative → 0 (1–2 stars)
- Neutral (3 stars) → removed

---

## 🧹 Preprocessing Pipeline

The following steps are applied to clean text data:

- Lowercasing text
- Removing punctuation
- Removing stopwords
- Tokenization
- Lemmatization

Output:
- Cleaned text used for feature extraction

---

## 🔤 Feature Extraction Methods

We use two different approaches:

### 1. TF-IDF (Traditional NLP)
- Converts text into sparse numerical vectors
- Used for baseline models

### 2. Word Embeddings
- Word2Vec or BERT embeddings
- Captures semantic meaning of text
- Used for deep learning models

---

## 🤖 Machine Learning Models

### 🔹 Baseline Model
- Logistic Regression / Naive Bayes
- Uses TF-IDF features

### 🔹 Advanced Model
- LSTM (or Transformer-based model)
- Uses word embeddings

---

## 📈 Evaluation Metrics

Both models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

### Model Comparison:
| Model               | Accuracy | F1-score |
|--------------------|----------|----------|
| Logistic Regression| XX%      | XX%      |
| LSTM / Transformer | XX%      | XX%      |

---

## 🔍 Insight Extraction

This project includes an interpretability layer that extracts:

### 🔹 Keywords
- Most frequent positive words
- Most frequent negative words

### 🔹 Phrases
- Common bigrams (e.g., "slow service", "great food")

### 🔹 Patterns
- Most common complaints (e.g., delivery issues)
- Most common praise (e.g., product quality)

### 🔹 Explanation System
Each prediction includes a reason:

Example:

Review: "The service was very slow"
Prediction: Negative
Reason: slow service