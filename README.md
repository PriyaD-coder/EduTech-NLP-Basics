# Task 15 – NLP Text Classification (Sentiment Analysis)

## Project Overview
This project performs **Sentiment Analysis** on IMDB Movie Reviews using Natural Language Processing (NLP).  
The goal is to classify movie reviews as **Positive** or **Negative** using Machine Learning.

---

## Objective
Build a complete NLP pipeline that includes:

- Text preprocessing (Tokenization, Stopword removal, Stemming)
- Feature extraction using TF-IDF
- Model training using Naive Bayes
- Model evaluation using classification metrics

This task demonstrates understanding of basic NLP and text classification.

---

## Dataset
Dataset used: IMDB Movie Reviews Dataset

The dataset contains movie reviews labelled as positive or negative.

### Columns:
| Column    | Description         |
|-----------|---------------------|
| review    | Movie review text   |
| sentiment | positive / negative |

An offline CSV file was used to avoid network issues while running the notebook.

---

##  Technologies Used
- Python  
- Pandas  
- NLTK  
- Scikit-learn  
- Jupyter Notebook  

---

##  Project Workflow

###  Text Preprocessing
Raw text cannot be used directly by machine learning models, so we cleaned and prepared it.

Steps performed:
- Removed HTML tags using Regular Expressions  
- Removed special characters and numbers  
- Converted text to lowercase  
- Tokenized sentences into words  
- Removed stopwords using NLTK  
- Applied Porter Stemming to reduce words to root form  

Example:
"Watching movies was amazing" → "watch movi amaz"

---

### Feature Extraction – TF-IDF
Machine learning models require numbers, not text.

We used TF-IDF (Term Frequency – Inverse Document Frequency) to convert text into numeric vectors.

TF-IDF gives:
- High importance → rare words
- Low importance → common words (like "the", "is")

---

###  Train-Test Split
Dataset was divided into:
- 80% Training Data
- 20% Testing Data

Training data → used to train model  
Testing data → used to evaluate performance

---

###  Model Training
Model used: Multinomial Naive Bayes

Why Naive Bayes?
- Very fast for text classification
- Works well with TF-IDF
- Ideal for sentiment analysis

---

###  Model Evaluation
Metrics used:
- Accuracy Score
- Confusion Matrix
- Precision
- Recall
- F1 Score

Expected Accuracy: 85% – 90%

---

##  Final Outcome
Successfully built a Movie Review Sentiment Classifier that can predict whether a review is Positive or Negative.

-<img width="1919" height="1024" alt="task15 1" src="https://github.com/user-attachments/assets/069efc49-6ec4-45d4-a5ed-cdf5b6f130b2" />
- <img width="1919" height="1023" alt="task15 2" src="https://github.com/user-attachments/assets/62e30fe7-c801-45e4-80b7-b28188a8d270" />

---

##  Interview Questions

### What is TF-IDF?
TF-IDF measures how important a word is in a document relative to the entire dataset.

Formula:
TF-IDF = Term Frequency × Inverse Document Frequency

---

##  Conclusion
This task demonstrates:
- NLP preprocessing
- Feature extraction using TF-IDF
- Machine learning for text classification
