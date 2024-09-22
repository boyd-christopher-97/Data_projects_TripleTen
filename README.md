# Data Projects (TripleTen)

This repository contains a collection of data science projects completed during the TripleTen course. Each project focuses on different data science techniques and models, showcasing various skills and methodologies.

## Table of Contents

1. [Project 1: Golden Age](./sprint_1/golden_age.ipynb)
2. [Project 2: Sentiment Analysis](#project-2-sentiment-analysis)
3. [Project 3: News Article Classification](#project-3-news-article-classification)
4. [Project 4: Sales Forecasting](#project-4-sales-forecasting)

---

## Golden Age

### Objective
The aim of this project is to investigate how the number of votes a title receives from IMDb users impacts its ratings. The assumption is that highly-rated shows (we will focus on TV shows, ignoring movies) released during the “Golden Age” of television also have the most votes.

### What Was Done
- Conducted an analysis to identify the "Golden Age" of cinema by examining the correlation between movie ratings and their release years.
- Cleaned the data by handling missing values and transforming categorical data.
- Applied visualization techniques to present the findings, including line plots for average ratings across decades
- Identified key periods with significant trends, and proposed insights into what contributed to the so-called "Golden Age" of cinema.

### Results
The research done confirms that highly-rated shows released during the "Golden Age" of television also have the most votes. While shows with score 4 have more votes than ones with scores 5 and 6, the top three (scores 7-9) have the largest number. The data studied represents around 94% of the original set so that we can be confident in our findings.

### Notebook
- [Notebook](./sprint_1/golden_age.ipynb)

---

## Project 2: Instacart Insights

### Objective
The mission is to clean up the data and prepare a report that gives insight into the shopping habits of Instacart customers.

### What Was Done
- Preprocess the data by doing the following: verify and fix data types, identify and fill in missing values, identify and remove duplicate values
- Verify that values in the 'order_hour_of_day' and 'order_dow' columns in the orders table are sensible (i.e. 'order_hour_of_day' ranges from 0 to 23 and 'order_dow' ranges from 0 to 6).
- Create a plot that shows how many people place orders for each hour of the day.
- Create a plot that shows what day of the week people shop for groceries.
- Create a plot that shows how long people wait until placing their next order, and comment on the minimum and maximum values.

-Is there a difference in 'order_hour_of_day' distributions on Wednesdays and Saturdays? Plot the histograms for both days on the same plot and describe the differences that you see.
-Plot the distribution for the number of orders that customers place (e.g. how many customers placed only 1 order, how many placed only 2, how many only 3, and so on…)
-What are the top 20 products that are ordered most frequently (display their id and name)?

### Results
Found how many items people typically buy in one order, the top 20 items that are reordered most frequently, and the top 20 items that people put in their carts first.

### Notebook
- [Notebook](./sprint_2/instacart_insights.ipynb)

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
