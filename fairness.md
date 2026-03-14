---
layout: default
title: Fairness Analysis
nav_order: 9
---

# Fairness Analysis

For our fairness analysis, we wanted to check whether the model performs worse for certain types of recipes. We focused on calorie level and split recipes into two groups using the median calorie value. Group X contains recipes with lower calories (below the median), and Group Y contains recipes with higher calories (above the median).

## Performance metric and Test Statistic
Since our model predicts a continuous rating, we evaluated performance using Mean Absolute Error (MAE). This measures the average difference between the predicted rating and the true rating. If the model is less accurate for one group, we would expect that group to have a larger MAE.

Our test statistic was the difference in MAE between the two groups:

T = MAE(high calorie) − MAE(low calorie)

## Perumutation Testing
To determine whether the observed difference could happen by chance, we ran a permutation test. We repeatedly shuffled the calorie group labels while keeping the model predictions fixed, and recalculated the difference in MAE each time. This gave us a distribution of differences we would expect if the model treated both groups the same.


## Results

<iframe src="/Modeling-Recipe-Ratings-Through-Structured-and-Text-Based-Feature-Engineering/Figure/Permutation Testing.html" width="800" height="250" frameborder="0" ></iframe>

The observed MAE values for the two groups were very similar, and the resulting p-value was fairly large. Because of this, we fail to reject the null hypothesis. In other words, we did not find evidence that the model performs meaningfully worse for high calorie recipes compared to low calorie ones.

We also repeated the same permutation test for sugar content and cooking time (quick vs slow recipes). In all three comparisons the error differences were very small, suggesting the model performs similarly across these recipe groups.

While this does not guarantee the model is perfectly fair across every possible subgroup, it suggests that calorie level alone does not create a meaningful performance gap in our model.
