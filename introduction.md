---
layout: default
title: Introduction
nav_order: 2
---

# Introduction

## Dataset Overview
The dataset our group chose to work with was one that contains recipes and ratings from food.com. Due to its massive size, we were provided with a dataset that was a subset of the original raw data. The recipes and ratings were provided in two separate CSV files and were ultimately merged, an action we will discuss further in our “Data Cleaning and Exploratory Data Analysis” section. The recipes dataset has 83782 rows, translating to 83782 unique recipes, and 12 columns:
- `name`: the name of the recipe
- `id`: the id number of the recipe
- `minutes`: the number of minutes needed to complete the recipe
- `contributor_id`: the id number of the person who contributed the recipe to the dataset
- `submitted`: the date in which the recipe was submitted (in YYYY-MM-DD format)
- `tags`: words/phrases associated with the recipe
- `nutrition`: nutritional information of the food in a list, listing calories, total fat, sugar, sodium, protein, and saturated fat (all but calories are represented as PDV, meaning “percentage of daily value”)
- `n_steps`: the number of steps it takes to complete the recipe
- `steps`: the steps required to complete the recipe, placed in a list
- `description`: a description of the recipe provided by the user
- `ingredients`: a list of ingredients used in the recipe
- `n_ingredients`: the number of ingredients used in the recipe
The ratings dataset has 731927 rows, translating to 731927 unique reviews, and has 5 columns:
- `user_id`: the id number of the user who submitted the review
- `recipe_id`: the id numbers of the recipe being reviewed
- `date`: the date the review was submitted (in YYYY-MM-DD format)
- `rating`: the rating given to the recipe
- `review`: comments provided by the reviewer
 

## Main Question
The main question our project focuses on is the following:
**To what extent do nutritional content, such as calories, and review-related variables shape the average rating of recipes?**

## Why This Matters
Readers of our website should care about this dataset and research question because it combines detailed nutritional information with review-related features from real Food.com users, allowing us to investigate what factors influence how recipes are rated. By examining both nutritional characteristics, such as calorie content, and aspects of user reviews, we can better understand what drives perceived recipe quality in a real-world setting. Our analysis explores whether factors like calories and review activity meaningfully shape the average rating of recipes, helping us evaluate common assumptions about food preferences. These insights are relevant for health-conscious cooks, recipe developers, and anyone interested in understanding how nutritional choices and user feedback relate to overall recipe satisfaction.

## Dataset Size
This is the size of our cleaned dataset:
- Number of rows: 231652
- Number of columns: 34

## Relevant Columns
Here are the columns used to answer our question:
- `calories` — the amount of calories in the recipe
- `minutes` — number of minutes it takes to complete the recipe
- `avg_rating` — the average rating of the recipe
- `n_steps`: the number of steps it takes to complete the recipe
- `n_ingredients`: the number of ingredients used in the recipe
- `sugar`: the PDV of sugar in the recipe
- `protein`: the PDV of protein in the recipe
- `carbohydrates`: the PDV of carbohydrates in the recipe
- `total_fat`: the PDV of total fat in the recipe
- `sodium`: the PDV of sodium in the recipe