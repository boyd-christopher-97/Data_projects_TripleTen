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
- [Notebook](./insurance_modeling.ipynb)
