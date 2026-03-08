---
layout: default
title: [Project Title]
---

# [Project Title]

### By [Reza Moghadam], [Dimas Molina], [Artien Voskanian], [Ann Nguyen]

[Write a short 2–3 sentence overview of the project and what it investigates.]

---

# Introduction

Dataset overview:  
[FILL IN short description of the dataset and what type of data it contains.]

Main question of the project:  
[FILL IN the one main question the project is centered around.]

Why this question matters:  
[FILL IN why someone should care about this dataset and question.]

Dataset size:
- Number of rows: [FILL IN]
- Number of columns: [FILL IN]

Relevant columns used in this project:

- `[column name]` — [short description]
- `[column name]` — [short description]
- `[column name]` — [short description]
- `[column name]` — [short description]
- `[column name]` — [short description]

---

# Data Cleaning and Exploratory Data Analysis

## Data Cleaning

[FILL IN description of the data cleaning steps.]

Possible things to mention:
- How missing values were handled
- Any rows that were removed
- Any new columns that were created
- Any transformations applied to existing columns
- Why these cleaning steps were necessary

Head of cleaned dataframe:

[INSERT TABLE OR SCREENSHOT OF CLEANED DATAFRAME HEAD]

---

## Univariate Analysis

[FILL IN short introduction explaining what variable distribution is being examined.]

PLOT PLACEHOLDER — UNIVARIATE DISTRIBUTION

[Insert at least one plotly plot showing the distribution of a single column.]

Interpretation:

[FILL IN 1–2 sentences describing what the distribution shows.]

---

## Bivariate Analysis

[FILL IN short explanation of what two variables are being compared.]

PLOT PLACEHOLDER — BIVARIATE RELATIONSHIP

[Insert at least one plotly plot showing the relationship between two columns.]

Interpretation:

[FILL IN 1–2 sentences explaining the trend or relationship in the plot.]

---

## Interesting Aggregates

TABLE PLACEHOLDER — GROUPED OR PIVOT TABLE

[Insert grouped summary table or pivot table.]

Explanation:

[FILL IN short explanation describing what the aggregate results show.]

---

# Assessment of Missingness

## NMAR Analysis

Column that may be NMAR:

`[column name]`

Reasoning:

[FILL IN explanation of why the missingness might be NMAR based on the data generating process.]

Additional data that could help explain the missingness:

[FILL IN what extra data would help determine whether the missingness could instead be MAR.]

---

## Missingness Dependency

Column with missing values being analyzed:

`[column name]`

Column where missingness appears dependent:

`[column name]`

Column where missingness appears not dependent:

`[column name]`

PLOT PLACEHOLDER — MISSINGNESS VISUALIZATION

[Insert plot related to missingness exploration.]

Permutation test results:

Dependent relationship:
- Test statistic: [FILL IN]
- p-value: [FILL IN]

Independent relationship:
- Test statistic: [FILL IN]
- p-value: [FILL IN]

Interpretation:

[FILL IN explanation of what the results suggest about missingness.]

---

# Hypothesis Testing

Question being tested:

[FILL IN the question your hypothesis test addresses.]

Null hypothesis:

[FILL IN null hypothesis.]

Alternative hypothesis:

[FILL IN alternative hypothesis.]

Test statistic:

[FILL IN test statistic.]

Significance level:

[FILL IN alpha value.]

P-value:

[FILL IN]

Conclusion:

[FILL IN conclusion while avoiding absolute claims.]

Justification:

[FILL IN why this hypothesis test and statistic were appropriate.]

PLOT PLACEHOLDER — HYPOTHESIS TEST VISUALIZATION

[Insert visualization related to hypothesis testing if included.]

---

# Framing a Prediction Problem

Prediction task:

[FILL IN what the model is trying to predict.]

Prediction type:

Regression or Classification

Response variable:

`[column name]`

Why this variable was chosen:

[FILL IN explanation.]

Information available at time of prediction:

- `[feature]`
- `[feature]`
- `[feature]`
- `[feature]`

Evaluation metrics:

- `[metric]`
- `[metric if additional]`

Why these metrics were chosen:

[FILL IN explanation.]

---

# Baseline Model

Baseline model type:

[FILL IN model name.]

Features used:

Quantitative features:
[FILL IN]

Ordinal features:
[FILL IN if applicable]

Nominal features:
[FILL IN if applicable]

Preprocessing steps:

[FILL IN description of scaling, encoding, or imputing.]

Baseline model performance:

- `[metric]`: [value]
- `[metric]`: [value]
- `[metric]`: [value]

Evaluation:

[FILL IN short explanation of whether the baseline model performed well and why.]

---

# Final Model

New features added:

- `[feature]`
- `[feature]`
- `[feature]`

Why these features should improve the model:

[FILL IN explanation based on the data generating process.]

Modeling algorithm used:

[FILL IN algorithm.]

Selected hyperparameters:

- `[parameter]`: [value]
- `[parameter]`: [value]
- `[parameter]`: [value]

Hyperparameter tuning method:

[FILL IN explanation of grid search or tuning method.]

Final model performance:

- `[metric]`: [value]
- `[metric]`: [value]
- `[metric]`: [value]

Improvement over baseline:

[FILL IN explanation.]

PLOT PLACEHOLDER — MODEL PERFORMANCE VISUALIZATION

[Insert model performance visualization if applicable.]

---

# Fairness Analysis

Groups compared:

Group X:  
[FILL IN]

Group Y:  
[FILL IN]

Evaluation metric used:

[FILL IN]

Null hypothesis:

[FILL IN]

Alternative hypothesis:

[FILL IN]

Test statistic:

[FILL IN]

Significance level:

[FILL IN]

P-value:

[FILL IN]

Conclusion:

[FILL IN fairness conclusion.]

PLOT PLACEHOLDER — PERMUTATION TEST DISTRIBUTION

[Insert permutation test visualization.]

Optional fairness comparison table:

| Group Comparison | Metric Group X | Metric Group Y | Ratio or Difference |
|---|---|---|---|
| [Comparison 1] | [value] | [value] | [value] |
| [Comparison 2] | [value] | [value] | [value] |
| [Comparison 3] | [value] | [value] | [value] |

---

# Final Takeaway

[FILL IN a short project summary describing the main insights from the analysis and modeling.]
