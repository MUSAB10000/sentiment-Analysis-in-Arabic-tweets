# Arabic Tweet Sentiment Analysis

## Problem Statement
The goal of this project is to build a machine learning model that accurately classifies Arabic tweets as **positive** or **negative**. The project involves data cleaning, preprocessing of Arabic text, feature extraction, model training, evaluation, and deployment of a web app for real-time sentiment prediction.

## Dataset Source
The dataset consists of four TSV files containing Arabic tweets:
- `train_Arabic_tweets_positive_20190413.tsv`
- `train_Arabic_tweets_negative_20190413.tsv`
- `test_Arabic_tweets_positive_20190413.tsv`
- `test_Arabic_tweets_negative_20190413.tsv`
**Source:** The data was obtained from https://www.kaggle.com/datasets/mksaad/arabic-sentiment-twitter-corpus

Each file includes two columns:
- **Sentiment Label:** The original sentiment label.
- **Arabic tweet:** The text of the tweet.

## Model Pipeline
The model pipeline follows these steps:
1. **Data Preprocessing:**
   - Cleaning and normalizing Arabic text (removing punctuations, diacritics, mentions, hashtags, and URLs).
   - Tokenizing the tweets and removing Arabic stopwords.
2. **Feature Extraction:**
   - Using `TfidfVectorizer` to convert text into numerical features.
3. **Classification:**
   - Applying a `LinearSVC` classifier to predict sentiment.

## Results
The model achieves an overall accuracy of approximately 78% on the test set. Evaluation metrics such as precision, recall, and F1 score indicate balanced performance between the positive and negative classes.

## Requirements
You can install these dependencies using the provided requirements.txt file.


