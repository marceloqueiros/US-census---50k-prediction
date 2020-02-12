# US census - 50k prediction
 Find out which features of the population are most related to income and predict who earns more or less than 50 thousand dollars.

# Introduction
This US Census dataset contains detailed but anonymized information for approximately 300,000 people.

The goal of this exercise is to model the information contained in the last column (42nd), i.e., whether a person makes more or less than 50,000 per year, from the information contained in the other columns. The exercise here consists of modeling a binary variable.

Work with Python (or R) to carry out the following steps:

1) Load the train and test files.

2) Perform an exploratory analysis on the data and create some relevant visualisations.

3) Clean, preprocess, and engineer features in the training data, with the aim of building a data set that a model will perform well on.

4) Create a model using these features to predict whether a person earns more or less than 50,000 per year. Here, the idea is for you to test a few different models, and see whether there are any techniques you can apply to improve performance over your first results.

5) Choose the model that appears to have the highest performance based on a comparison between reality (the 42nd variable) and the model’s prediction.

6) Apply your model to the test file and measure its real performance on it (same method as above).

The goal of this exercise is not to create the best or the purest model, but rather to describe the steps you took to accomplish it.

Explain areas that may have been the most challenging for you.

Find clear insights on the profiles of the people that make more than 50,000 / year. For example, which variables seem to be the most correlated with this phenomenon?

# Development
See ipynb file.

# Conclusion

It’s obvious that features like age, education, sex, country of birth, race, capital gains, capital losses and dividends from stocks are very related to the income, as it can be seen in this project.

In this project, it is important to have good accuracy for both classes. As the test dataset has more lines for one of the classes, if the accuracy of this class is optimal, the algorithm will perform well in this data, just like the first extra tree algorithm (95% general accuracy but about 50% of accuracy for the least represented class). So, I prefer an algorithm like XBGClassifier with 92.3% accuracy but with good accuracy for both classes.

The dataset that I trained with was balanced with SMOTE.
