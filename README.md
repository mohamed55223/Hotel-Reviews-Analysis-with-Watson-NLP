Here is a possible README file for the provided code:

# Sentiment Analysis on Hotel Reviews

This repository contains code for sentiment analysis on hotel reviews. The code performs various tasks including loading the reviews, extracting frequently mentioned hotel aspects, extracting document and sentence sentiment, identifying nouns that drive sentiment, and conducting targeted sentiment analysis.

## Table of Contents
1. [Load the reviews](#loadData)
2. [Extract frequently mentioned hotel aspects](#extractNouns)
3. [Extract document and sentence sentiment](#extractSentiment)
4. [Identify nouns that drive sentiment](#sentenceSentiment)
5. [Targets sentiment analysis](#targetedSentiment)
6. [Summary](#summary)

## Prerequisites
Before running the code, you need to ensure you have the following dependencies installed:
- pandas
- matplotlib
- watson_nlp

## Usage
1. Clone the repository or download the source code.
2. Make sure you have the required dependencies installed.
3. Open the Jupyter Notebook `Hotel_Review_Analysis.ipynb` in your preferred environment.
4. Follow the code sections step by step to load the reviews, extract hotel aspects, analyze document and sentence sentiment, identify nouns driving sentiment, and perform targeted sentiment analysis.
5. Adjust the code and parameters as needed to suit your specific use case.

<a id="loadData"></a>
## 1. Load the reviews
This section loads the hotel reviews into a DataFrame. The reviews are stored in a CSV file named `"hotel_reviews.csv"`. The data set contains four columns: hotel name, review date, review title, and review text. The code loads the data into a DataFrame using the Pandas library.

<a id="extractNouns"></a>
## 2. Extract frequently mentioned hotel aspects
In this section, the code extracts the most frequently mentioned aspects (nouns) in the reviews for each hotel. This helps to understand what aspects guests are talking about in their reviews. The code uses the Watson Natural Language Processing pre-trained syntax model to extract the most frequently used nouns from the reviews. Lemmatized versions of the nouns are stored to create more accurate statistics.

<a id="extractSentiment"></a>
## 3. Extract document and sentence sentiment
This section focuses on extracting sentiment for the complete reviews and individual sentences. The code uses the Watson Natural Language Processing sentiment model to extract sentiment at the document and sentence levels. The sentiment extraction is performed using a pre-trained sentiment model for English.

<a id="sentenceSentiment"></a>
## 4. Identify nouns that drive sentiment
Here, the code identifies the most frequently used nouns in sentences with positive or negative sentiment. It creates dataframes for positive and negative sentiment nouns and visualizes the most frequent nouns using bar charts for each hotel.

<a id="targetedSentiment"></a>
## 5. Targeted Sentiment Analysis
In this section, the code performs targeted sentiment analysis using the *Targets Sentiment Extraction Workflow* provided by Watson Natural Language Processing. This workflow extracts targets and the sentiment expressed towards each target term for each sentence in the input document. It can handle multiple targets with different sentiments in one sentence.

## Summary
This repository provides code for sentiment analysis on hotel reviews. It allows you to load the reviews, extract frequently mentioned aspects, analyze document and sentence sentiment, identify nouns driving sentiment, and perform targeted sentiment analysis. Feel free to explore the code and adapt it to your specific needs.



