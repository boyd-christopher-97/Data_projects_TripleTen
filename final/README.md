## Project 12: Churn Forecast

### Objective
The goal of this project is to develop a machine learning model to predict customer churn for **Interconnect**, a telecom operator. If a customer is predicted to churn, the company will offer them promotional codes and special plan options to retain their business. The primary metric for model performance is the AUC-ROC score, with an additional metric of accuracy.

### What Was Done

- **Data Overview**:
  - The dataset contains **7043 entries**, with **26.5%** of the entries representing customers who have churned, indicating a class imbalance.
  - No outliers were present, and all data types were adjusted for modeling.

- **Data Preprocessing**:
  - Combined multiple data sources (contract, personal, internet, phone) into a single DataFrame.
  - Performed feature engineering, including modifications to the `BeginDate` and `EndDate` columns to help the model identify churn behavior.
  - Addressed target leakage by dropping the `BeginDate` column and replacing it with derived features like `days_active` and `months_active`.

- **Model Training**:
  - Applied **XGBoost**, **LightGBM**, and **CatBoost** models for churn prediction.
  - Tuned model hyperparameters using GridSearchCV to optimize performance for each model.
  - Feature engineering and one-hot encoding were crucial in enhancing model performance and addressing the class imbalance.

- **Model Evaluation**:
  - The **XGBoost** model was selected as the final model, optimized using GridSearchCV over 3 folds.
  - Best parameters: `colsample_bytree: 1`, `learning_rate: 0.1`, `max_depth: 6`, `n_estimators: 200`, `subsample: 1`.
  - The final **AUC-ROC score** achieved on the test set was **0.90**, exceeding the target of 0.88.

### Key Steps
1. **Feature Engineering**: Adjusted `BeginDate` and `EndDate`, derived new features like `days_active`, and handled target leakage.
2. **Hyperparameter Tuning**: GridSearchCV was used to fine-tune XGBoost, achieving optimal model performance.
3. **Model Selection**: Compared multiple models, selecting **XGBoost** based on its superior performance.

### Challenges and Solutions
- **Target Leakage**: The `BeginDate` column caused target leakage, which was addressed by replacing it with derived features (`days_active` and `months_active`).
- **Class Imbalance**: Managed class imbalance with careful feature engineering and by selecting appropriate model parameters.

### Results
- **Final Model**: The final model is **XGBoost**, achieving an AUC-ROC score of **0.90** on the test set.
- **Business Application**: The model allows Interconnect to predict customer churn effectively and implement targeted marketing strategies, such as offering promotional codes or special plan options to retain customers.

   ### Notebook
- [Notebook](./churn_forecast.ipynb)
