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

Naive Random Oversmpling Results:
![This is an image](https://github.com/Jahill17/Credit_Risk_Analysis/blob/main/Screenshots/Credit_risk_resampling-RandomOversampling.png)

SMOTE Oversampling Results:
![This is an image](https://github.com/Jahill17/Credit_Risk_Analysis/blob/main/Screenshots/Credit_risk_resampling-SMOTEOversampling.png)

Undersampling Results:
![This is an image](https://github.com/Jahill17/Credit_Risk_Analysis/blob/main/Screenshots/Credit_risk_resampling-Undersampling.png)

SMOTEENN Combination Sampling Results:
![This is an image](https://github.com/Jahill17/Credit_Risk_Analysis/blob/main/Screenshots/Credit_risk_resampling-CombinationOverUnderSampling.png)

Balanced Random Forest Classifier Results:

Easy Ensemble AdaBost Classifier Results:


## Summary
Generally sensitivity is more important than precision when it comes to analyzing risk and default rates for prospective loan candidates.  Sensitivity is the percentage of true positives, whereas precision is the meausre of how reliable a positive classification is.  A high sensitivity means that given percentage of individuals will actually test positive.  A low precision is indicative of a large number of false positives, inversely a high precision is indicative of a small number of false positives. Sensitivity helps rule out individuals when the candidate result is bad (negative) for the prospective candidate.  With the above information in mind, precision is not as important as long as the potential defaults are appropriately flagged.

... algorithms had fairly low precision rate for high risk individuals.  The highest precision rate is the...  This implies that of all the customers marked as high risk, approximately... were actually high risk.

The algorithm with the highest sensitivithy is the... The model implies that... of the time the high risk individuals are appropriately marked as high risk individuals. The...model had the next highest sensitivity at...

Another tool to look at is the balanced accuracy score.  The balanced accuracy score implies how correct the model is, meaning that of all the predictions how many of the predictions were classified correctly.  The model with the highest acccuracy score is the... Based on this result the... model should be the one we choose because it has the highest sensitivity, highest precision, and also has high accuracy.
