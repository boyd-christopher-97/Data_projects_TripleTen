## Project 5: Plan Recommendation

### Objective
The goal of this project is to develop a machine learning model for the mobile carrier **Megaline** that recommends the optimal plan for their subscribers: **Smart** or **Ultra**. The model is trained on subscriber behavior data, aiming for an accuracy threshold of 0.75 on the test dataset.

### What Was Done
- **Data Overview**:
  - The dataset contains monthly behavior information for each user, including the number of calls, total minutes, messages, internet usage (in MB), and the plan each user was on (`Ultra` or `Smart`).
  - The target variable is the `is_ultra` column (1 for Ultra, 0 for Smart).

- **Data Preparation**:
  - Split the data into training, validation, and test sets using an 80-10-10 split ratio.
  - Ensured that the split provided a balanced distribution of plan types across the training, validation, and test sets.

- **Model Development**:
  - Investigated the performance of various classification models, including:
    - **Logistic Regression**
    - **Random Forest**
    - **Decision Tree**
    - **K-Nearest Neighbors (KNN)**
  - Performed hyperparameter tuning using grid search and cross-validation to maximize model performance.
  - Evaluated the models based on accuracy on the validation set to select the best-performing one for the test set.

- **Model Evaluation**:
  - The final model achieved an accuracy score of **0.80** on the test set, surpassing the project threshold of 0.75.
  - The **Random Forest Classifier** performed the best, with a balanced accuracy across both `Ultra` and `Smart` plan recommendations.
  
- **Sanity Check**:
  - Performed additional testing to ensure the model's stability, confirming that its predictions generalized well to unseen data.

### Results
- **Best Model**: The Random Forest Classifier achieved the highest accuracy, correctly predicting plan recommendations for 80% of the test data.
- **Hyperparameter Findings**:
  - Increasing the number of trees in the forest and fine-tuning the maximum depth improved accuracy.
  - Logistic Regression and KNN underperformed compared to tree-based methods.
- **Insights**:
  - Users with higher internet usage and more calls were more likely to be assigned to the **Ultra** plan.
  - The model provided actionable insights that could assist Megaline in recommending plans to new users based on their monthly behavior.
 
  ### Notebook
- [Notebook](./plan_recommendation.ipynb)
