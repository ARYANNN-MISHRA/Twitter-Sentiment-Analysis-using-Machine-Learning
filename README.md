# Twitter Sentiment Analysis using Machine Learning 

## Overview
This project implements a Machine Learning-based sentiment analysis system to classify tweets into **Positive** and **Negative** sentiments. The workflow includes data preprocessing, text vectorization using TF-IDF, model training, and evaluation using a large-scale Twitter dataset. 

It demonstrates an end-to-end Natural Language Processing (NLP) pipeline for analyzing social media text and extracting sentiment-based insights.

---
# Twitter Sentiment Analysis

A sentiment classification project analyzing 1.6 million tweets to predict positive or negative sentiment, comparing multiple machine learning models.

## Overview
This project uses the Sentiment140 dataset to build and evaluate text classification models that predict tweet sentiment (positive/negative). The pipeline covers text preprocessing, TF-IDF feature extraction, multi-model training, and performance comparison.

## Dataset
- **Source:** Sentiment140 (1.6M labeled tweets)
- **Labels:** Binary — Negative (0), Positive (1)
- **Split:** 80% train / 20% test (1.28M train, 320K test)

## Approach
1. **Data Cleaning:** Removed neutral-class rows, mapped polarity labels, normalized text casing
2. **Feature Extraction:** TF-IDF vectorization with unigrams + bigrams (top 5000 features)
3. **Model Training:** Trained and compared three classifiers:
   - Bernoulli Naive Bayes
   - Logistic Regression
   - Linear SVM
4. **Evaluation:** Accuracy, precision, recall, F1-score, and confusion matrix

## Results

| Model | Accuracy |
|---|---|
| **Logistic Regression** | **79.54%** |
| Linear SVM | 79.53% |
| Bernoulli Naive Bayes | 76.65% |

Logistic Regression and Linear SVM performed near-identically and both outperformed Naive Bayes by ~3 percentage points.

## Visualizations
- Confusion matrix for the best-performing model
- Word clouds highlighting frequent terms in positive vs. negative tweets

## Tools Used
Python, Pandas, Scikit-learn, TF-IDF, Matplotlib, Seaborn, WordCloud

## Files
- `TwitterSentiment.ipynb` — full notebook with code, outputs, and visualizations
## Problem Statement
Social media platforms generate millions of opinions every day, making manual analysis of this data impossible. The objective of this project is to automatically determine whether a tweet expresses a positive or negative sentiment using Machine Learning classification techniques.

---

## Dataset
**Dataset:** [Sentiment140](http://help.sentiment140.com/for-students)  
**Total Tweets:** 1,600,000  

The dataset features a binary sentiment classification model based on the following labels:
*   **0** → Negative
*   **4** → Positive (converted to binary `1` during preprocessing)

**Columns Used:**
*   `Sentiment Label`
*   `Tweet Text`

---

## Technologies Used
*   **Language:** Python
*   **Environment:** Jupyter Notebook
*   **Libraries:** Pandas, Scikit-learn
*   **Techniques:** TF-IDF Vectorizer, Bernoulli Naive Bayes

---

## Workflow

### 1. Data Loading
*   Loaded the Sentiment140 dataset.
*   Selected the relevant text and label columns.
*   Renamed dataset fields for easier access.

### 2. Data Preprocessing
*   Removed unnecessary columns.
*   Converted the original sentiment labels into standard binary classes (`0` and `1`).
*   Prepared and cleaned the text data for feature extraction.

### 3. Feature Engineering
Applied **TF-IDF (Term Frequency-Inverse Document Frequency) Vectorization** to convert the raw tweets into numerical vectors suitable for ML models.
*   **Maximum Features:** 5,000
*   **N-gram Range:** (1, 2)

### 4. Modeling
*   **Algorithm:** Bernoulli Naive Bayes
*   The model was trained on the extracted TF-IDF features and evaluated on a held-out test dataset of **320,000 tweets**.

---

## Results
The Bernoulli Naive Bayes model achieved consistent performance across all major classification metrics.

| Metric | Score |
| :--- | :--- |
| **Accuracy** | 76.65% |
| **Precision** | 0.77 |
| **Recall** | 0.77 |
| **F1 Score** | 0.77 |

---

## Key Skills Demonstrated
1   Natural Language Processing (NLP)
2  Machine Learning Classification
3  Text Preprocessing & Data Cleaning
4  Feature Engineering (TF-IDF Vectorization)
5  Model Training & Evaluation
6  Data Analysis
