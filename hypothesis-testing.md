---
layout: default
title: Hypothesis Testing
nav_order: 5
---

# Hypothesis Testing

## Question
Nutrition is often a consideration when people choose and evaluate recipes. We investigated <b>whether the amount of calories has any effect on how users rate recipes</b>, specifically, whether indulgent, high-calorie recipes receive different ratings than lighter alternatives. 
High-calorie recipes are defined as those whose calorie count exceeds the median calorie value across all recipes in the dataset and low calories as those below the median.
To examine this, we conducted a permutation test under the following conditions:

## Null Hypothesis
The mean recipe average rating is the same for high-calories and low-calories recipes.

## Alternative Hypothesis
The mean recipe average rating differs between high-calories recipes and low-calories recipes.

## Test Statistic
The difference in mean between average rating of high-calories recipes and low-calories recipes.

## Significance Level
0.05

## Method
To ensure each recipe was represented once, ratings were aggregated to the recipe level by computing each recipe's average rating before grouping. A permutaion test was performed 5000 times, shuffling the high/low calorie group labels each iteration to build an empirical null distribution.

<iframe src="/Modeling-Recipe-Ratings-Through-Structured-and-Text-Based-Feature-Engineering/Figure/Cal_hypTesting_Step4.html" width="100%" height="600" frameborder="0"></iframe>

## Conclusion
The <b>observed difference</b> in mean rating between high-calorie and low-calorie recipes was <b>–0.0084</b> (denoted as verticle black dashed line), indicating that high-calorie recipes were rated very slightly lower on average. However, with a <b>p-value of 0.0624</b> > 0.05, we <b>fail to reject the null hypothesis</b>. This suggests that the observed difference is within the range of what could arise by chance alone. Therefore, we do not have sufficient evidence to conclude that caloric content is associated with recipe ratings.

