# Customer Sentiment Analysis

## Overview

A sentiment classification system built on the IMDB movie reviews dataset.
Compared Logistic Regression and Naive Bayes models to find the best approach
for transforming raw customer text into Positive/Negative predictions.

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
- *Techniques:* TF-IDF Vectorization, Logistic Regression, Naive Bayes, Text Preprocessing
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

### 3. Model Training & Comparison

- Split data: *80% train / 20% test*
- Trained and compared *Logistic Regression* vs *Naive Bayes*
- Evaluated on Accuracy, Precision, Recall, and F1 Score

-----

## Results

|Metric   |Logistic Regression|Naive Bayes|
|---------|-------------------|-----------|
|Accuracy |*0.8867*         |0.8538     |
|Precision|*0.8816*         |0.8512     |
|Recall   |*0.8951*         |0.8589     |
|F1 Score |*0.8883*         |0.8554     |

✅ *Logistic Regression outperformed Naive Bayes on all metrics*

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
   git clone https://github.com/sirishaxx/Customer-Sentiment-Analysis.git
   
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
