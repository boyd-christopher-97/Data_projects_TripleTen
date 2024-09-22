# Data Projects (TripleTen)

This repository contains a collection of data science projects completed during the TripleTen course. Each project focuses on different data science techniques and models, showcasing various skills and methodologies.

## Table of Contents

1. [Project 1: Churn Prediction](#project-1-churn-prediction)
2. [Project 2: Sentiment Analysis](#project-2-sentiment-analysis)
3. [Project 3: News Article Classification](#project-3-news-article-classification)
4. [Project 4: Sales Forecasting](#project-4-sales-forecasting)

---

## Basic Python: Project

### Objective
The aim of this project is to investigate how the number of votes a title receives from IMDb users impacts its ratings. The assumption is that highly-rated shows (we will focus on TV shows, ignoring movies) released during the “Golden Age” of television also have the most votes.

### What Was Done
- Conducted an analysis to identify the "Golden Age" of cinema by examining the correlation between movie ratings and their release years.
- Cleaned the data by handling missing values and transforming categorical data.
- Applied visualization techniques to present the findings, including line plots for average ratings across decades
- Identified key periods with significant trends, and proposed insights into what contributed to the so-called "Golden Age" of cinema.

### Results
The research done confirms that highly-rated shows released during the "Golden Age" of television also have the most votes. While shows with score 4 have more votes than ones with scores 5 and 6, the top three (scores 7-9) have the largest number. The data studied represents around 94% of the original set so that we can be confident in our findings.

### Files
- [Notebook](./sprint_1/golden_age.ipynb)

---

## Project 2: Sentiment Analysis

### Objective
To build a sentiment analysis model that classifies IMDb movie reviews as either positive or negative, enhancing the platform’s recommendation system.

### What Was Done
- Used logistic regression with TF-IDF features for classification.
- Preprocessed text data using NLTK and spaCy (tokenization, stopword removal, and lemmatization).
- Achieved an F1 score of 0.88, surpassing the initial target.

### Results
The model improved the recommendation accuracy by accurately categorizing user reviews.

### Screenshots
![Sentiment Analysis Confusion Matrix](./images/sentiment_confusion_matrix.png)

---

## Project 3: News Article Classification

### Objective
To classify news articles into predefined topics (science, politics, entertainment, and sports) using a neural network.

### What Was Done
- Built a neural network for topic classification using text preprocessing techniques.
- Used CountVectorizer to transform text data into numerical format.
- Achieved 95% accuracy on the test set with k-fold cross-validation.

### Results
The model accurately classified news articles across various topics, ensuring robust performance.

### Screenshots
![News Classification Model Architecture](./images/news_model.png)

---

## Project 4: Sales Forecasting

### Objective
To build a time series forecasting model for predicting future sales based on historical data, enabling better business planning.

### What Was Done
- Built a Prophet model to forecast sales trends.
- Created features like lag values and rolling averages to improve the forecast.
- Evaluated the model using RMSE and MAE metrics.

### Results
The model provided actionable insights for sales trends, helping the business optimize inventory management.

### Screenshots
![Sales Forecasting Plot](./images/sales_forecasting_plot.png)

---

## Further Improvements

1. Implementing real-time prediction capabilities in projects.
2. Exploring ensemble methods and advanced models for improved accuracy.
3. Building API integrations for easier deployment of the models.

---

### Contact

Feel free to check out my other projects and contributions on my GitHub profile: [boyd-christopher-97](https://github.com/boyd-christopher-97).
