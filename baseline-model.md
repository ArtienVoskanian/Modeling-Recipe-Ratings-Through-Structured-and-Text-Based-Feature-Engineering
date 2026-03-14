---
layout: default
title: Baseline Model
nav_order: 7
---

# Baseline Model

## Model Type
Linear Regression   

## Features Used
We used 9 recipe-level features: `minutes`, `n_steps`, `n_ingredients`, `calories`, `sugar`, `protein`, `carbohydrates`, `total_fat`, and `sodium`. All 9 features were quantitative, with 0 ordinal features and 0 nominal features.

## Preprocessing
Because all features were numeric, we did not need to use one-hot encoding or ordinal encoding. We handled missing values using median imputation and standardized the features before fitting the model.

## Performance
- `MAE`: 0.4653
- `RMSE`: 0.6410
- `R^2`: 0.00016

## Evaluation
Our baseline model was a Linear Regression model predicting avg_rating using 9 recipe-level features: minutes, n_steps, n_ingredients, calories, sugar, protein, carbohydrates, total_fat, and sodium. All 9 of these features were quantitative, with 0 ordinal and 0 nominal features. Because they were all numeric, we did not need to use one-hot encoding or ordinal encoding. We handled missing values with median imputation and standardized the features before fitting the model. We used this model as a simple baseline so that we could compare it with more advanced models later.
