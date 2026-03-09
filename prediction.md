---
layout: default
title: Prediction Problem
nav_order: 6
---

# Framing a Prediction Problem

## Prediction Task
We aim to predict the average rating of a recipe based on both its intrinsic 
characteristics and user-generated content. Rather than restricting features 
to those available at posting time, this model leverages all available 
information about a recipe, including user reviews, to estimate how a recipe 
will be rated. This framing is better suited for retrospective rating 
estimation, for example, surfacing predicted ratings for recipes with 
missing ratings rather than pre-interaction prediction.

## Prediction Type
This is a <b>regression</b> problem, as average rating is a continuous variable on a 1–5 scale rather than a discrete category.

## Response Variable
The response variable is `average_rating`, computed as the mean of all individual ratings submitted for each recipe. This aggregation ensures each recipe is represented by a single target value.

## Features Available at Prediction Time
Features include `minutes`, `n_steps`, and `n_ingredients`, which capture 
the recipe's complexity and preparation demands, as well as nutritional 
features: `calories`, `sugar`, `protein`, `carbohydrates`, `total_fat`, and 
`sodium`. The final model additionally incorporates text features derived 
from user `review` text. While reviews are not available prior to user 
interaction, including them improves predictive performance and aligns with 
the retrospective framing of this task.

## Evaluation Metrics
We evaluate model performance using RMSE, MAE, and R². Since ratings are 
bounded on a 1–5 scale, prediction errors carry real interpretive weight. 
RMSE captures this by penalizing larger errors more heavily through its 
squared term. MAE complements RMSE by reporting the average error in the 
same units as the rating scale, making it more intuitive to interpret and 
more robust to outliers. Together, RMSE and MAE provide both a sensitive 
and robust picture of prediction error. R² is included as a relative measure 
of model fit, indicating how much of the variance in average rating is 
explained by the model's features, which helps contextualize raw error values.


