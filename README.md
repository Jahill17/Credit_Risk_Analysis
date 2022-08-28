# Credit_Risk_Analysis

## Supervised Machine Learning Analysis Overview
The primary objective of this project is to use machine learning models to analyze credit risk, with the goal of a quicker and more reliable loan experience.  Using the machine learning language tools I was able to identify appropriate candidates for loans.  Identifying the proper candidates could result in a decrease in default rate on a financial institutions loans.


## Resources
- LoanStats_2019Q1.csv (Provided Dataset)
- Python
- Jupyter Notebook
- Google Colab
- NumPy
- SciKit-Learn


## Results
**Summary of all machine learning tools**:
![This is an image](https://github.com/Jahill17/Credit_Risk_Analysis/blob/main/Screenshots/ML_Summary_Results.png)

**Naive Random Oversmpling Results**:
![This is an image](https://github.com/Jahill17/Credit_Risk_Analysis/blob/main/Screenshots/Credit_risk_resampling-RandomOversampling.png)

**SMOTE Oversampling Results**:
![This is an image](https://github.com/Jahill17/Credit_Risk_Analysis/blob/main/Screenshots/Credit_risk_resampling-SMOTEOversampling.png)

**Undersampling Results**:
![This is an image](https://github.com/Jahill17/Credit_Risk_Analysis/blob/main/Screenshots/Credit_risk_resampling-Undersampling.png)

**SMOTEENN Combination Sampling Results**:
![This is an image](https://github.com/Jahill17/Credit_Risk_Analysis/blob/main/Screenshots/Credit_risk_resampling-CombinationOverUnderSampling.png)

**Balanced Random Forest Classifier Results**:
![This is an image](https://github.com/Jahill17/Credit_Risk_Analysis/blob/main/Screenshots/Credit_risk_ensemble-BalancedRandomForest.png)

**Easy Ensemble AdaBost Classifier Results**:
![This is an image](https://github.com/Jahill17/Credit_Risk_Analysis/blob/main/Screenshots/Credit_risk_ensemble-EasyEnsembleAdaBoost.png)

## Summary
Generally sensitivity is more important than precision when it comes to analyzing risk and default rates for prospective loan candidates.  Sensitivity is the percentage of true positives, whereas precision is the meausre of how reliable a positive classification is.  A high sensitivity means that given percentage of individuals will actually test positive.  A low precision is indicative of a large number of false positives, inversely a high precision is indicative of a small number of false positives. Sensitivity helps rule out individuals when the candidate result is bad (negative) for the prospective candidate.  With the above information in mind, precision is not as important as long as the potential defaults are appropriately flagged.

All of the algorithms had low precision rate for high risk individuals.  The highest precision rate is the Easy Ensemble AdaBoost at 7%.  This implies that of all the customers marked as high risk, approximately 7% were actually high risk.  In contract, all of the models have a perfect 100% for low risk individuals; this means that any customer marked as low risk is actually low risk.

Since precision does not distinguish much between the models it is beneficial to look at sensitivity.  The algorithm with the highest sensitivithy is the Easy Ensemble AdaBoost at 91%. The model implies that 91% of the time the high risk individuals are appropriately marked as high risk individuals. The SMOTEENN Combination model had the next highest sensitivity at 70%.

Another tool to look at is the balanced accuracy score.  The balanced accuracy score implies how correct the model is, meaning that of all the predictions how many of the predictions were classified correctly.  The model with the highest acccuracy score is the Easy Ensemble AdaBoost at 92%, followed by the Balanced Random Forest at 79%. Based on the results of the differents models, the Easy Ensemble AdaBoost model should be used since it has the highest sensitivity, highest precision, and also has high accuracy.  The combination of all three data points makes the Easy Ensemble AdaBoost model the best choice.
