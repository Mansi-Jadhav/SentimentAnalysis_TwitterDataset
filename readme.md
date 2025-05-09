# Twitter Sentiment Analysis Using NLP and Machine Learning

**Goal:**
This project applies Natural Language Processing (NLP) and traditional machine learning techniques to perform sentiment analysis on Twitter data. 

**Dataset:**
Labelled dataset with approximately 27000 tweets from Twitter and their labels.
 
## Overview of Steps:

**Data Loading & Parsing:**
Reads a tab-separated Twitter dataset, extracting tweet text and sentiment labels (e.g., positive, negative).

**Text Preprocessing:**
Cleans tweets using regular expressions - removing punctuation, special characters, converting text to lowercase.
Tokenizes and lemmatizes text using NLTK’s WordNetLemmatizer.

**Feature Engineering:**
Extracts text features using TfidfVectorizer to transform raw tweets into numerical representations suitable for modeling.

**Model Building:**
Implements a classification pipeline using LinearSVC (Support Vector Classifier) wrapped with NLTK’s SklearnClassifier.

**Evaluation:**
Evaluates the model using cross-validation and standard metrics such as precision, recall, F1-score, and accuracy.
Performs error analysis to identify common misclassifications.

**Testing on Unseen Data:**
Applies the trained model on unseen test tweets to assess generalization.
