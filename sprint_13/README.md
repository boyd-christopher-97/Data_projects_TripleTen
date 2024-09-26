## Project 10: Order Prediction

### Objective
The objective of this project is to develop a machine learning model to predict the number of taxi orders for the **Sweet Lift Taxi** company in the next hour. This prediction will help the company attract more drivers during peak hours, ensuring that supply meets demand. The goal is to achieve an RMSE score on the test set of no more than 48.

### What Was Done

- **Data Preparation**:
  - Resampled the dataset by one-hour intervals and handled any missing values.
  - Created additional time-based features such as the hour of the day, day of the week, and lag features to help the model identify trends and patterns.

- **Model Development**:
  - Trained and compared multiple models, including:
    - **Auto Regression**
    - **Moving Average**
    - **Prophet**

- **Model Evaluation**:
  - Used the RMSE (Root Mean Squared Error) metric to evaluate the models.
  - Split the dataset into 90% for training and 10% for testing.
  - Fine-tuned the models to ensure the RMSE on the test set was below the threshold of 48.

### Results
Prophet is a robust forecasting library that effectively handles outliers and missing data, which contributes to its strong performance in terms of RMSE. In our analysis, we observed significant fluctuations towards the end of the dataset, particularly within the 6-month cycle, which the Prophet model captured well. Given these factors, I recommend that Sweet Lift Taxi use the Prophet model to predict the number of taxi orders for the next hour.
  ### Notebook
- [Notebook](./order_prediction.ipynb)

