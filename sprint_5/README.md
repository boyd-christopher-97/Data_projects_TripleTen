## Project 4: Game Success 

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
- [Notebook](./game_success.ipynb)
