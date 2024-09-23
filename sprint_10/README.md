## Project 7: Gold Prediction

### Objective
The goal of this project is to develop a machine learning model that predicts the amount of gold recovered from ore. This model will help **Zyfra**, a company specializing in efficiency solutions for heavy industry, optimize their production process and eliminate unprofitable parameters.

### What Was Done
- **Data Preparation**:
  - Cleaned and preprocessed data on gold extraction and purification.
  - Handled missing values and performed feature engineering to select important features for the model.
  
- **Data Analysis**:
  - Conducted exploratory data analysis (EDA) to examine the relationships between the features and the target variable (gold recovery).
  - Visualized key metrics, including recovery efficiency at different stages of the production process.

- **Model Development**:
  - Trained multiple machine learning models including:
    - Linear Regression
    - Random Forest
  - Evaluated model performance 
  
- **Model Tuning**:
  - Fine-tuned hyperparameters for the final model to optimize predictive accuracy.
  - Selected the best model based on cross-validation results.

### Results
Using the data on extraction and purification, the random forest model performs best and predicts the amount of gold recovered from gold ore. Using hyperparameters n_estimators: 30 best_depth: 10 allowed me to narrow it down to 8.8% on the best validation set and 7.7% on the final rf test set. Furthermore, a percentage difference of 7.7% is generally low and tells us the model's predictions are close to the target. Within the sanity check, I found a 10.8% final smape on the train set and 9% on test which indicates the random forest model performs better.

  ### Notebook
- [Notebook](./gold_prediction.ipynb)
