## Project Overview
The dataset pertains to a Teaching Assistant (TA) evaluation problem in the education domain, where we are tasked with predicting the performance of teaching assistants based on various factors. 

The problem is a classification problem.

Dataset Size: 151 records and 6 columns.

Target Column: Performance (binary classification).

Features:

Whether the TA is a native English speaker (binary).

Course instructor (categorical).

Course (categorical).

Summer or regular semester (binary).

Class size (numerical).

Class attribute (categorical).

## Objectives
The main objective is to build a model that can accurately predict the performance of teaching assistants based on the provided features.

## Data Preprocessing & Feature Engineering
Column Naming: The dataset didn’t contain column names, so we added them based on the metadata provided in the text file.

Missing Values: No missing values were found.

Duplicates: 41 duplicated records were identified and removed.

### Univariate Analysis:
Count plots for the binary features (Performance, Summer/Regular semester, Native English speaker).

Histograms for categorical features (Course, Class size, Course instructor).

Skewness: Skewness of data was calculated.

Outliers: No outliers were detected using box plots.

Correlation: Correlation was checked using the corr() function, and multicollinearity was assessed using a heatmap.

### Modelling
Train-Test Split: Split data into training and testing sets to avoid overfitting and ensure robust model performance.

Feature Scaling: Applied scaling to speed up training and improve model performance.

Model Comparison: Evaluated several classification algorithms:

Decision Tree Classifier: Accuracy = 64.5%

Random Forest Classifier: Accuracy = 70.9%

Gradient Boosting Classifier: Accuracy = 74.19%

XGBoost Classifier: Accuracy = 70.9%

Despite feature transformation, the results remained consistent across models.

### Hyperparameter Tuning: After tuning the Gradient Boosting model, the accuracy dropped to 29.03%, which was much lower than the initial performance.

## Challenges Faced
Column names were in a separate file, and the data description was in a text file.

Best accuracy of 74.19% was achieved with Gradient Boosting, but hyperparameter tuning led to a significant drop in accuracy.

Despite different model approaches, performance stagnated after tuning.

## Conclusion
The dataset was properly explored, and after testing various models, Gradient Boosting Classifier emerged as the best performing model, achieving an accuracy of 74.19%. 
However, hyperparameter tuning was not beneficial in this case, as it caused a performance drop.

