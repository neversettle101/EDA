# Data preprocessing 

1. Convert categorical data to numerical data → pd.get_dummies
2. What do you do when your data is null values?
    1. Check which feature is more/less correlated to the data with missing values. Add average values to the missing data

# Learnings

## Feature Scaling
1. Standardization
Data standardization is a technique used when features in a dataset exhibit significant differences in their ranges or are measured in different units. It involves centering the values around the mean and adjusting the distribution to have a unit standard deviation such that the mean becomes 0 and standard deviation becomes 1

Z-score formula
$$ Z = \frac{{X - \mu}}{{\sigma}} $$

Algorithms to be used in : PCA, Clustering, KNN, SVM, Regression

2. Normalization
Min-Max Scaling
Min-max scaling is very often simply called ‘normalization.’ It transforms features to a specified range, typically between 0 and 1. The formula for min-max scaling is:

Xnormalized = X – Xmin / Xmax – Xmin

Q. Do I need feature scaling?
Q. If yes: Which to choose? https://www.datacamp.com/tutorial/normalization-in-machine-learning
Some additional tips:
1. If range of features is known then use normalization eg. image classification
2. If there are outliers in the data use standardization
Mostly standardization is used