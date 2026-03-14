# Flavors, Features, and Feedback: A Data Science Approach to Recipe Ratings

## Main Question

> **To what extent do nutritional content, such as calories, and review-related variables shape the average rating of recipes?**

---

## Why This Matters

This project combines recipe nutrition information with ratings from real Food.com users to study how nutritional qualities relate to public satisfaction, offering insight into the balance between health and taste in a real-world setting.

Many people assume that higher-calorie recipes are more enjoyable while lower-calorie options are less appealing. By comparing average ratings across calorie groups, we can test whether that belief is actually supported by user behavior. The findings are relevant to health-conscious cooks, recipe creators, and anyone trying to make better food choices without sacrificing enjoyment.

---

## Dataset

This dataset contains recipes and ratings from [Food.com](https://www.food.com/), originally scraped and published by Majumder et al. in *Generating Personalized Recipes from Historical User Preferences* (Bodhisattwa Prasad Majumder, Shuyang Li, Jianmo Ni, Julian McAuley).

**Cleaned dataset size:**
- Rows: 231,652
- Columns: 34

---

## Report Sections

1. **Introduction** — Background, dataset overview, and main question
2. **EDA** — Exploratory data analysis of nutritional and rating distributions
3. **Missingness** — Analysis of missing data patterns and dependencies
4. **Hypothesis Testing** — Permutation test comparing ratings across calorie groups
5. **Prediction Problem** — Framing the modeling task and evaluation metric
6. **Baseline Model** — Initial model using core features
7. **Final Model** — Improved model with engineered features and tuning
8. **Fairness Analysis** — Evaluation of model performance across recipe subgroups
9. **Conclusion** — Summary of findings and implications

## Website
https://artienvoskanian.github.io/Modeling-Recipe-Ratings-Through-Structured-and-Text-Based-Feature-Engineering/

## Authors

*Reza Moghadam, Dimas Molina, Ann Nguyen, Artien Voskanian*

