# Module 17 Assignment 17.1 - Comparing Classifiers

## Summary

This repository contains an analysis of a UCI Machine Learning provided marketing data set for Portugese banking marketing campaigns. Some summary findings:

* People are more likely to buy financial products if they feel that the economy is doing well.
* People don't like to recieve telemarketing calls on mobile phones.
* Customers are more likely to accept an offer for a term deposit account if they haven't been called with an offer in a while.
* Customers are more receptive in the months of March, May, and June.

## Analysis

The [Jupyter notebook](practical_application_3.ipynb) contains the data analysis and recommendations. The data was cleaned to reduce the number of rows with `unknown` values which removed about 1/4 of the data, but provided a better basis for comparison between customers. The data was also highly imbalanced with only 12.66% of customers in the subscribing class. The baseline model that always predicts rejection scored 0.87339 accuracy. Always predicting "no" is not very useful. The model parameters were tuned to optimize ROC AUC and a logistic regression with feature selection produced the best results.

The repository also contains the [Prompt](prompt_III.ipynb) notebook with some introductory examination prompted by the course.
