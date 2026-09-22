# Video Views Prediction

A machine learning regression project for predicting Day-30 video views using early video engagement data.

## Problem

The goal is to predict `target_day30_views` using information available shortly after a video is posted.

## Features

The final model uses two features:

- `duration`
- `day5_plays`

`day5_plays` is extracted from the engagement data for Day 5 after posting.

## Models Tested

Several regression models were evaluated using 5-fold cross-validation:

- Linear Regression
- Ridge Regression
- Huber Regression
- Theil-Sen Regression
- RANSAC Regression
- Random Forest
- Extra Trees
- Gradient Boosting
- XGBoost

## Final Model

Huber Regression was selected based on the lowest cross-validation RMSE among the tested models.

**5-Fold CV RMSE: 66,094.45**

## Submission

The final model was trained on the complete training dataset and used to generate predictions for the competition test set.

The resulting file is:

`submission.csv`

## Tools

- Python
- Pandas
- NumPy
- Scikit-learn
- Kaggle
- Jupyter Notebook
