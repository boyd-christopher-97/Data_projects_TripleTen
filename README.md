# Data Projects (TripleTen)

This repository contains a collection of data science projects completed during the TripleTen course. Each project focuses on different data science techniques and models, showcasing various skills and methodologies.

## Table of Contents

1. [Project 1: Churn Prediction](#project-1-churn-prediction)
2. [Project 2: Sentiment Analysis](#project-2-sentiment-analysis)
3. [Project 3: News Article Classification](#project-3-news-article-classification)
4. [Project 4: Sales Forecasting](#project-4-sales-forecasting)

---

## Project 1: Churn Prediction

### Objective
The goal of this project was to build a machine learning model to predict customer churn, helping businesses identify at-risk customers and improve retention strategies.

### What Was Done
- Developed an XGBoost model for customer churn prediction.
- Data preprocessing, feature engineering, and hyperparameter tuning using GridSearchCV.
- Achieved an ROC AUC score of 0.9018 on the test set.

### Results
The model successfully identified 90% of high-risk customers, allowing targeted marketing strategies for retention.

### Screenshots
![Churn Prediction ROC Curve](./images/churn_roc_curve.png)

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
