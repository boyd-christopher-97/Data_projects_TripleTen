## Project 9: Car Valuation 

### Objective
The goal of this project is to develop a machine learning model for **Rusty Bargain**, a used car sales service, to determine the market value of a car based on historical data. The model needs to provide accurate predictions, fast inference, and efficient training times.

### What Was Done

- **Data Preparation**:
  - Cleaned the dataset by handling missing values, formatting date columns, and encoding categorical variables.

- **Model Development**:
  - Trained and compared multiple models including:
    - **Linear Regression**: Used as a baseline for sanity checks.
    - **Decision Tree**: Tuned depth and split criteria.
    - **Random Forest**: Tuned number of trees and depth.
    - **LightGBM**: Tuned boosting rounds and learning rate.
    - Optionally trained **CatBoost** and **XGBoost** with hyperparameter tuning.

- **Model Evaluation**:
  - Compared models based on RMSE (Root Mean Squared Error) to evaluate prediction accuracy.
  - Measured training time and prediction speed for each model, balancing performance and efficiency.

### Results
When comparing the model's training times, the gradient boosting methods demonstrate significantly faster performance compared to other models like Random Forest, Decision Tree, and Linear Regression. Among these, LightGBM not only offers the highest accuracy, but also has a great prediction speed.
Although the prediction time for LightGBM is slightly slower compared to other models, the difference in time is marginal and does not significantly impact the overall performance. Therefore, given its accuracy and training speed, I recommend using the LightGBM model for this task.

  ### Notebook
- [Notebook](./car_valuation.ipynb)
