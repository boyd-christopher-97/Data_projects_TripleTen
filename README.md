# Data Projects (TripleTen)

This repository contains a collection of data science projects completed during the TripleTen course. Each project focuses on different data science techniques and models, showcasing various skills and methodologies.

## Table of Contents

1. [Project 1: Golden Age](./sprint_1/golden_age.ipynb)
2. [Project 2: Instacart Insights](./sprint_2/instacart_insights.ipynb)
3. [Project 3: Plan Profitability](./sprint_3/plan_profitability.ipynb)
4. [Project 4: Game Success](./sprint_5/game_success.ipynb)
5. [Project 5: Plan Recommendation](./sprint_7/plan_recommendation.ipynb)
6. [Project 6: Profit Evaluation](./sprint_9/profit_evaluation.ipynb)
7. [Project 7: Gold Prediction](./sprint_10/gold_prediction.ipynb)
8. [Project 8: Insurance Modeling](./sprint_11/insurance_modeling.ipynb)
9. [Project 9: Car Valuation](./sprint_12/car_valuation.ipynb)
10. [Project 10: Car Valuation](./sprint_13/order_prediction.ipynb)
11. [Project 9: Car Valuation](./sprint_14/car_valuation.ipynb)


---

## Project 1: Golden Age

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

## Project 3: Plan Profitability Analysis

### Objective
This project focuses on analyzing the profitability of two prepaid plans offered by the telecom operator Megaline: **Surf** and **Ultimate**. The company aims to determine which plan brings in more revenue to adjust the advertising budget accordingly.

### What Was Done
- Collected and prepared data from 500 Megaline clients, including information about calls, messages, and internet usage.
- Calculated the monthly revenue for each client by accounting for the fixed plan costs and extra charges for minutes, messages, and data exceeding the plan limits.
- Conducted statistical analysis to compare the profitability of the two plans:
  - Described customer behavior in terms of minutes used, text messages sent, and data consumed.
  - Performed hypothesis testing to check if:
    - The average revenue differs between users of the **Surf** and **Ultimate** plans.
    - The average revenue in the NY-NJ area differs from other regions.

### Results
- The analysis revealed that:
  - Users of the **Ultimate** plan typically generate more revenue than those on the **Surf** plan due to the higher monthly charge.
  - There was a statistically significant difference in the average revenue between the two plans.
  - The average revenue from users in the NY-NJ area did not significantly differ from users in other regions.

### Hypothesis Testing
- **Null Hypothesis**: The average revenue from **Ultimate** plan users is the same as from **Surf** plan users.
- **Alternative Hypothesis**: The average revenue from **Ultimate** plan users is different from **Surf** plan users.
- **Test Method**: T-test was used to compare the means of the two groups.

### Notebook
- [Notebook](./sprint_3/plan_profitability.ipynb)

### Conclusion
This project provided valuable insights into the revenue generated by the two prepaid plans offered by Megaline. The analysis concluded that the **Ultimate** plan, with its higher monthly charge and lower rates for overage usage, typically yields more revenue compared to the **Surf** plan. This information will help the company make informed decisions on how to allocate advertising resources.


---

## Project 4: Game Success Analysis

### Objective
In this project, the goal is to identify patterns that determine whether a video game succeeds or fails. The analysis is based on historical sales data, user and professional reviews, genres, and platforms. The findings will help forecast game success and plan advertising campaigns for the year 2017.

### What Was Done
- **Data Preprocessing**:
  - Cleaned and converted data columns (e.g., column names were made lowercase, missing values were handled, and correct data types were applied).
  - Replaced placeholder values like TBD (to be determined) with appropriate values or left them as is depending on the context.
  - Calculated total global sales for each game across all regions.

- **Data Analysis**:
  - Analyzed the number of game releases by year to identify trends.
  - Compared sales across different platforms, focusing on platforms with the highest total sales and identifying the platforms that were once popular but are now obsolete.
  - Investigated sales by genre and determined which genres are most and least profitable.
  - Created a user profile for each region (NA, EU, JP), identifying the top platforms, genres, and analyzing the effect of ESRB ratings on sales.

- **Statistical Analysis**:
  - Conducted hypothesis testing to evaluate:
    - Whether the average user ratings of Xbox One and PC platforms are the same.
    - Whether the average user ratings for Action and Sports genres are different.
  - Applied T-tests to verify the hypotheses and interpreted the results.

### Results
- **Platform Analysis**:
  - Identified the leading platforms in sales, including those experiencing growth and decline.
  - Box plots for global sales showed significant differences in sales across platforms.
  - Some platforms, like PlayStation and Xbox, dominated global sales while others, like the Wii, experienced a sharp decline.

- **Review Impact**:
  - The analysis of user and professional reviews for a selected platform revealed correlations between reviews and sales. User reviews were found to have a moderate correlation with sales, while professional reviews had a stronger impact on sales figures.

- **Genre Trends**:
  - Action and Shooter genres were identified as the most profitable, while genres like Puzzle and Adventure were found to have lower sales.
  - Regional preferences for genres were distinct, with Japan showing a preference for Role-Playing games compared to North America and Europe.

- **Hypothesis Testing**:
  - **Hypothesis 1**: The average user ratings for Xbox One and PC platforms are statistically similar.
    - The null hypothesis could not be rejected, indicating no significant difference in the average user ratings for these platforms.
  - **Hypothesis 2**: The average user ratings for Action and Sports genres differ.
    - The null hypothesis was rejected, confirming a statistically significant difference in the average user ratings for Action and Sports games.

### Conclusion
This project provided valuable insights into the gaming industry's dynamics, focusing on how different platforms, genres, and regions affect game success. The analysis highlighted key factors that contribute to high sales, such as platform popularity, genre preferences, and user reviews, helping to guide marketing strategies for future game releases.

### Notebook
- [Notebook](./sprint_5/game_success.ipynb)
---

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
- [Notebook](./sprint_7/plan_recommendation.ipynb)

## Project 6: Profit Evaluation
---
### Objective
The goal of this project is to help the **OilyGiant mining company** identify the best region for developing a new oil well. Using geological data from three regions, we built a predictive model to estimate the volume of oil reserves and evaluate the potential profit and risks.

### What Was Done
- **Data Preprocessing**: 
  - Analyzed geological data from three regions, prepared it for model training, and split it into training and validation sets.
- **Model Training**:
  - Built a linear regression model to predict the volume of reserves.
  - Evaluated the model's performance using RMSE and compared predicted reserves across regions.
- **Profit Calculation**:
  - Defined the profitability threshold for new wells.
  - Selected the top 200 wells based on predicted reserve volumes.
  - Calculated the expected profit for each region based on a $100 million budget.
- **Risk Evaluation**:
  - Applied the Bootstrapping technique with 1000 samples to calculate the distribution of profits.
  - Determined the 95% confidence interval and calculated the risk of loss for each region.
  
### Results
After training and testing the model of the three regions, region one had the highest profit potential; however, its rmse value was roughly 30x higher, which gave more room for error and higher risk of loss. From the start, I could see that region three would have the highest risk of loss, and this was confirmed after the bootstrapping method. Overall, the risk of loss is low in the second region, and it is apparent that it contains the highest average profit. For these reasons, I suggest the second region to develop oil wells.

  ### Notebook
- [Notebook](./sprint_9/profit_evaluation.ipynb)
---

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
- [Notebook](./sprint_10/gold_prediction.ipynb)

---

## Project 8: Insurance Modeling

### Objective
The objective of this project is to evaluate how **Sure Tomorrow Insurance** can use Machine Learning to address multiple business problems, including customer similarity identification, benefit prediction, and data protection.

### What Was Done

- **Task 1: Customer Similarity**:
  - Built a model to identify customers who are similar to a given customer, helping the company's marketing team target specific customer groups more effectively.
  
- **Task 2: Benefit Prediction**:
  - Developed a classification model to predict whether a new customer is likely to receive insurance benefits.
  - Compared the trained model’s performance to a dummy model, proving the trained model significantly outperforms a non-trained baseline.

- **Task 3: Linear Regression for Benefit Count**:
  - Built a linear regression model to predict the number of insurance benefits a new customer might receive based on features like gender, age, salary, and number of family members.

- **Task 4: Data Protection**:
  - Implemented a data masking (data obfuscation) technique to protect clients' personal data without affecting the model’s performance.
  - Demonstrated that the obfuscated data preserved the quality of machine learning predictions while securing sensitive information.

### Results
With obfuscation, we developed a data transformation algorithm that makes it hard to recover personal information if data falls into the wrong hands. In the final portion of the project, we found obfuscation does not affect our rmse and r2 values.
  ### Notebook
- [Notebook](./sprint_11/insurance_modeling.ipynb)

---

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
- [Notebook](./sprint_12/car_valuation.ipynb)

---
## Project 10: Order Prediction

### Results
Prophet is a robust forecasting library that effectively handles outliers and missing data, which contributes to its strong performance in terms of RMSE. In our analysis, we observed significant fluctuations towards the end of the dataset, particularly within the 6-month cycle, which the Prophet model captured well. Given these factors, I recommend that Sweet Lift Taxi use the Prophet model to predict the number of taxi orders for the next hour.
  ### Notebook
- [Notebook](./sprint_13/order_prediction.ipynb)
