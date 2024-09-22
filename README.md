# Data Projects (TripleTen)

This repository contains a collection of data science projects completed during the TripleTen course. Each project focuses on different data science techniques and models, showcasing various skills and methodologies.

## Table of Contents

1. [Project 1: Golden Age](./sprint_1/golden_age.ipynb)
2. [Project 2: Sentiment Analysis](./sprint_2/instacart_insights.ipynb)
3. [Project 3: News Article Classification](./sprint_3/plan_profitability.ipynb)
4. [Project 4: Sales Forecasting](#project-4-sales-forecasting)

---

## Project 2: Golden Age

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
