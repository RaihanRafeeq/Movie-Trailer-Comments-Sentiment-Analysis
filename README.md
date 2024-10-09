## Movie-Trailer-Comments-Sentiment-Analysis
This project focuses on building a sentiment analysis model for Manglish (Malayalam written in English) comments from YouTube movie trailers. The dataset consists of comments labeled into five categories.
# Project Overview
This project aims to build a sentiment analysis model to classify Manglish (Malayalam written in English) comments from YouTube movie trailers. The dataset includes comments categorized into the following sentiment labels:

Positive
Negative
Mixed_feelings
unknown_state
not-malayalam
The goal of the project is to train a machine learning model that can accurately predict the sentiment of unseen Manglish comments. The LSTM-based neural network architecture is used for this task, given its proficiency in handling sequential text data.

# Dataset
The training dataset is in TSV format with two columns: text (the comment) and category (the sentiment label).
The test dataset also follows the TSV format, but it includes an additional id column that can be ignored during processing.
Class Distribution
The class distribution in the training and test datasets shows an imbalance, with some categories like Positive being more frequent than others, such as Mixed_feelings and unknown_state.

# Model Architecture
The sentiment classifier uses an LSTM (Long Short-Term Memory) model due to its effectiveness in capturing long-term dependencies in text data. The architecture involves:

Tokenization and padding of text sequences.
Embedding layers to convert words into vectors.
LSTM layers to capture the sequential nature of text.
Dense layers for classification into the five sentiment categories.
# Steps to Run
Preprocess the data: Tokenize the comments, apply padding, and encode the labels.
Train the model: The LSTM model is trained on the labeled dataset.
Evaluate: The model is tested on the test dataset, and evaluation metrics such as accuracy, precision, recall, and F1-score are generated.
# Evaluation Metrics
The performance of the model is evaluated using:

Accuracy
Precision
Recall
F1-score
