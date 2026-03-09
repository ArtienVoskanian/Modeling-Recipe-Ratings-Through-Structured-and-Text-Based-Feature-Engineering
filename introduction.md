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
How does the average rating for “low-sugar” recipes compare to the average rating for “high-sugar” recipes?

## Why This Matters
Readers of our website should care about our dataset and our question because it combines recipe nutrition information with ratings from real Food.com users, allowing us to study how nutritional qualities relate to public satisfaction. This makes the dataset especially useful for understanding the balance between health and taste in a real-world setting. Our question about low-sugar versus high-sugar recipe ratings is important because many people assume that recipes with more sugar are more enjoyable, while lower-sugar recipes are less appealing. By comparing average ratings across these groups, we can test whether that belief is actually supported by user behavior and provide insight that is relevant to health-conscious cooks, recipe creators, and anyone trying to make better food choices without giving up enjoyment.

## Dataset Size
This is the size of our cleaned dataset:
- Number of rows: 231652
- Number of columns: 34

## Relevant Columns
Here are the columns used to answer our question:
- `sugar` — the PDV of sugar in the recipe
- `high_sugar` — Boolean indicating whether or not the recipe's level of sugar is above the median value of sugar
- `avg_rating` — the average rating of the recipe
