Overview

This project implements a Machine Learning-based sentiment analysis system to classify tweets into Positive and Negative sentiments. The workflow includes data preprocessing, text vectorization using TF-IDF, model training, and evaluation using a large-scale Twitter dataset.

The project demonstrates an end-to-end Natural Language Processing (NLP) pipeline for analyzing social media text and extracting sentiment-based insights.

Problem Statement

Social media platforms generate millions of opinions every day. Manually analyzing this data is impractical.

The objective of this project is to automatically determine whether a tweet expresses a positive or negative sentiment using Machine Learning techniques.

Dataset

Dataset: Sentiment140

1,600,000 tweets
Binary sentiment classification
Labels:
0 → Negative
4 → Positive (converted to binary)

Dataset columns used:

Sentiment Label
Tweet Text
Technologies Used
Python
Pandas
Scikit-learn
TF-IDF Vectorizer
Bernoulli Naive Bayes
Jupyter Notebook
Workflow
1. Data Loading
Loaded the Sentiment140 dataset.
Selected relevant columns.
Renamed dataset fields.
2. Data Preprocessing
Removed unnecessary columns.
Converted sentiment labels into binary classes.
Prepared text data for feature extraction.
3. Feature Engineering

Applied TF-IDF Vectorization

Maximum Features: 5000
N-gram Range: (1,2)

This converts tweets into numerical vectors suitable for Machine Learning models.

Model

Bernoulli Naive Bayes

The model was trained on TF-IDF features and evaluated on a held-out test dataset.

Results
Metric	Score
Accuracy	76.65%
Precision	0.77
Recall	0.77
F1 Score	0.77

Test Dataset Size:

320,000 tweets

Key Skills Demonstrated
Data Cleaning
Text Preprocessing
Feature Engineering
TF-IDF Vectorization
Machine Learning
Natural Language Processing
Model Evaluation
Classification
Data Analysis
