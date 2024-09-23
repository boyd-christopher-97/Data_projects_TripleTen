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
- [Notebook](./profit_evaluation.ipynb)
