# Mini Project: ML - Predictive Model Development and Analysis

## Data Source
[Comprehensive Diabetes Clinical Dataset(100k rows)](https://www.kaggle.com/datasets/priyamchoksi/100000-diabetes-clinical-dataset), from Kaggle.

## Methodology
After importing the data and an initial exploration to understand it, the data was cleaned and feature engineering was performed to be able to use the data in Machine Learning models. The object is creating the best model able to predict if a patient has diabetes or not based on the given data. Three differernt models were tested, both with the original data and scaled data, providing the following results:
- K-Nearest Neighbors:
    - With original data:
        - Accuracy score: 0.95
        - True positives / negatives: 950 / 18110
        - False positives / negatives: 793 / 144
    - With scaled data:
        - Accuracy score: 0.95
        - True positives / negatives: 937 / 18118
        - False positives / negatives: 806 / 136
- Decision Tree:
    - With original data:
        - Accuracy score: 0.97
        - True positives / negatives: 1202 / 18254
        - False positives / negatives: 541 / 0
    - No need to test scaled data, as decision tree gives the same result with original or scaled data.
- Logistic Regression:
    - With original data:
        - Accuracy score: 0.96
        - True positives / negatives: 1137 / 18083
        - False positives / negatives: 606 / 171
    - With scaled data:
        - Accuracy score: 0.96
        - True positives / negatives: 1144 / 18092
        - False positives / negatives: 599 / 162

## Conclusions
The best model for this case is the Decision Tree with 3 levels of depth, since it's the one with the best accuracy score, and doesn't give any false negatives in the test group.