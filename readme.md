# Spam SMS Classification using NLP

## Overview

This project implements a spam SMS classification pipeline using natural language processing (NLP) techniques. It covers data preprocessing, exploratory data analysis, feature extraction, model building, and evaluation, all demonstrated in a Jupyter Notebook.

## Repository Structure

```
├── data
│   └── Spam_SMS.csv        # Raw dataset of SMS messages labeled as spam or ham
├── notebooks
│   └── nlp-study.ipynb     # Jupyter Notebook with analysis and model implementation
└── README.md               # Project overview and instructions
```

## Dataset

The dataset used is the "Spam SMS Collection" from Kaggle, containing SMS messages labeled as "spam" or "ham". To run the notebook, download `Spam_SMS.csv` and place it in the `data/` directory.

## Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```
2. **(Optional) Create a virtual environment**:
   ```bash
   python3 -m venv venv
   source venv/bin/activate      # On Windows: venv\Scripts\activate
   ```
3. **Install dependencies**:
   ```bash
   pip install pandas numpy matplotlib seaborn nltk wordcloud scikit-learn vaderSentiment scipy
   ```

## Usage

1. **Download NLTK data**:
   ```python
   import nltk
   nltk.download('stopwords')
   nltk.download('punkt')
   ```
2. **Run the notebook**:
   ```bash
   jupyter notebook notebooks/nlp-study.ipynb
   ```

## Features

- **Data Preprocessing**: Tokenization, stopword removal, stemming, and text cleaning.
- **Exploratory Data Analysis (EDA)**: Distribution of spam vs. ham, word frequency analysis, and word clouds.
- **Feature Extraction**: Bag-of-Words and TF-IDF vectorization.
- **Model Building**: Training and comparison of Naive Bayes, Logistic Regression, and SVM classifiers.
- **Evaluation**: Accuracy, confusion matrix, classification report (precision, recall, F1-score), and ROC-AUC.

## Contributing

Contributions are welcome! Please open an issue to discuss proposed changes or submit a pull request.

