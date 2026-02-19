# Tweet Sentiment Analysis with TF-IDF & BERT

This project builds a tweet sentiment classification pipeline using both traditional NLP methods and transformer-based models. It combines Twitter API data collection, large-scale dataset analysis, and model comparison within a single notebook.

The goal is to compare TF-IDF-based models with BERT-based representations for sentiment prediction.

## Project Structure
  
  #### tweet_sentiment_analysis.ipynb – Main notebook containing:
  
  •	Twitter API data collection
  
  •	Large dataset loading
	
  •	Exploratory analysis
	
  •	TF-IDF feature extraction
	
  •	BERT embeddings
	
  •	Model training and comparison

## Workflow
  
  #### 1.	Twitter API Data Collection
  The notebook first defines functions to collect recent tweets from Twitter API v2 for a list of queries and saves them into tweets.csv. It handles rate limits and skips queries already stored.  ￼
	
  #### 2.	Load Twitter Dataset
  A large labelled dataset of 1.6 million tweets (training.1600000.processed.noemoticon.csv) is loaded with columns like sentiment target, tweet ID, date, and text.  ￼
	
  #### 3.	Exploratory Data Analysis (EDA)
  The dataset’s shape, columns, and basic info (number of records and data types) are printed to inspect the data before modeling.  ￼
	
  #### 4.	Text Feature Preparation
  (In later cells) tweets are cleaned and converted into numerical text features using:
	•	TF-IDF vectorization
	•	BERT embeddings
  These allow machine learning models to work with text data.
	
  #### 5.	Model Training & Evaluation
  Models are trained on the extracted features and evaluated to compare performance between TF-IDF-based models and BERT-based representations.
