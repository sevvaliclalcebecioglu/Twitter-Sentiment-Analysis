# Twitter Sentiment Analysis using Python

This project focuses on analyzing the sentiment of tweets using Natural Language Processing (NLP) and Machine Learning techniques. The goal is to classify tweets into different sentiment categories and evaluate the performance of multiple classifiers.

---

## 📌 Project Overview

Twitter is a widely used social media platform where users freely express their opinions. These opinions may include offensive language or hate speech. In this project, tweets are analyzed and classified based on their sentiment using machine learning models.

The dataset used in this project was obtained from Kaggle and contains labeled tweets categorized into three classes:
- **0**: Hate Speech  
- **1**: Offensive Language  
- **2**: Neither  

---

## 🗂 Dataset Description

The dataset includes the following important columns:

- `tweet`: Text content of the tweet  
- `class`: Target label representing sentiment category  

Only these two columns were used in model training to avoid data leakage.

---

## ⚙️ Data Preprocessing

The following preprocessing steps were applied:

- Converting text to lowercase
- Removing URLs, mentions, hashtags, and punctuation
- Removing stopwords
- Tokenization and text normalization

These steps help reduce noise and improve model performance.

---

## ☁️ Word Cloud Visualization

A Word Cloud function was created to visualize the most frequent words in tweets.  
Separate word clouds were generated for different sentiment classes to better understand commonly used terms.

---

## 🧠 Sentiment Analysis with TextBlob

In addition to machine learning models, **TextBlob** was used to analyze sentiment polarity and subjectivity of sample tweets.

Example:
```python
from textblob import TextBlob

text = "allyhaaaaa lemmie eat oreo amp dishes oreo lol"
blob = TextBlob(text)
blob.sentiment
