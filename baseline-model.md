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

The baseline model achieved an `MAE` of 0.4653, meaning that its predictions were off by about 0.465 rating units on average. Its `RMSE` was 0.6410, which is larger than the MAE and suggests that some predictions had noticeably larger errors. Its `R^2` was 0.00016, which is essentially zero, meaning the model explained almost none of the variation in recipe ratings and performed only slightly better than simply predicting the mean rating every time.
Overall, this baseline had very limited predictive power, but it served as a useful reference point for comparing more advanced models.