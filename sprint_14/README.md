## Project 11: Review Classification

### Objective
The goal of this project is to develop a machine learning model that automatically classifies IMDb movie reviews as positive or negative for **The Film Junky Union**. The model should achieve an F1 score of at least 0.85 to ensure accurate detection of negative reviews, assisting the platform's review filtering system.

### What Was Done

- **Data Preprocessing**:
  - Loaded and inspected the dataset (`imdb_reviews.tsv`).
  - Preprocessed the text data by cleaning, tokenizing, and converting text into numerical vectors using TF-IDF (Term Frequency-Inverse Document Frequency).
  - Performed exploratory data analysis (EDA) to check for class imbalances between positive and negative reviews.

- **Model Training**:
  - Trained three different models for text classification:
    1. **Logistic Regression**
    2. **Random Forest**
    3. **Gradient Boosting**
  - Evaluated the models using accuracy, precision, recall, and F1 score, with a focus on achieving the target F1 score of 0.85.
  
- **Model Testing**:
  - Tested the models on the test dataset to validate performance.
  - Composed and classified a few custom reviews using each model to test real-world applicability.

- **Evaluation**:
  - Compared the models' performance on the test set and custom reviews.
  - Provided explanations for performance differences between the models.

 ### Results
 Overall, preprocessing libraries such as NLTK and spaCy have proven to be effective, achieving an F1 score of 0.88, which indicates their capability to accurately categorize unrecognized reviews. Additionally, the combination of TF-IDF and logistic regression was successful in determining the sentiment of reviews, effectively classifying them as either positive or negative.

  ### Notebook
- [Notebook](./review_classification.ipynb)
