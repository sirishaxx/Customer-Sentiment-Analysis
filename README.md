# Customer Sentiment Analysis

## Overview

A sentiment classification system built on the IMDB movie reviews dataset.
The project transforms raw customer text into Positive/Negative predictions
using NLP preprocessing and Logistic Regression.

-----

## Problem Statement

Manually reading thousands of reviews is not scalable. This project automates
sentiment classification to extract business insights from large volumes of
unstructured text data.

-----

## Dataset

- *Source:* IMDB Dataset (via GitHub — laxmimerit/All-CSV-ML-Data-Files)
- *Columns:* review, sentiment (positive / negative)
- *Size:* ~50,000 reviews

-----

## Tools & Technologies

- *Language:* Python
- *Libraries:* pandas, NumPy, NLTK, scikit-learn, Matplotlib
- *Techniques:* TF-IDF Vectorization, Logistic Regression, Text Preprocessing
- *Platform:* Google Colab

-----

## Approach

### 1. Text Preprocessing

- Removed special characters using regex
- Converted text to lowercase
- Removed English stopwords using NLTK
- Applied cleaning pipeline across all 50,000 reviews

### 2. Feature Extraction

- Used *TF-IDF Vectorizer* with max_features=5000
- Mapped sentiment labels: positive → 1, negative → 0

### 3. Model Training

- Split data: *80% train / 20% test*
- Trained a *Logistic Regression* classifier

### 4. Evaluation & Visualization

- Achieved *88.67% accuracy* on the test set
- Plotted Sentiment Distribution (Positive vs Negative) using Matplotlib

-----

## Results

|Metric      |Value              |
|------------|-------------------|
|Model       |Logistic Regression|
|Accuracy    |*88.67%*         |
|Dataset Size|~50,000 reviews    |
|Features    |5,000 (TF-IDF)     |

-----

## Sample Predictions

python
predict_sentiment("This product is amazing")  # → Positive
predict_sentiment("Worst experience ever")    # → Negative


-----

## Project Structure


customer-sentiment-analysis/
│
├── Customer_Sentiment_Analysis.ipynb   # Main Colab notebook
├── README.md
└── requirements.txt


-----

## How to Run

1. Clone the repository
   
   bash
   git clone https://github.com/sirishaxx/customer-sentiment-analysis.git
   
1. Open the notebook in Google Colab or Jupyter
1. Run all cells — dataset loads automatically from the URL

-----

## Course Context

*Florida Atlantic University* — NLP & Information Retrieval | Aug – Dec 2025

-----

## Author

*Sirisha Gadde*  
MS Computer Science, Florida Atlantic University  
[LinkedIn](https://linkedin.com/in/sirisha-gadde) • [GitHub](https://github.com/sirishaxx)
