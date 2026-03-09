---
layout: default
title: Missingness
nav_order: 4
---

# Assessment of Missingness

## NMAR Analysis
In this dataset, we observed missing values in "description", "reviews" and "ratings" columns. 

Review missingness is likely NMAR (Not Missing At Random). The decision to leave a written review depends heavily on the user’s experience. Specifically, users with strong opinions, either positive or negative, are more inclined to write reviews, while neutral experiences often go unreported. Because the probability of a review being missing depends on the unobserved review content itself, no observed variable fully explains this pattern.

## Missingness Dependency
Recipe description and rating missingness are likely MAR (Missing At Random). The presence of recipe descriptions depends on author engagement, an observed and measurable variable. Similarly, rating missingness is influenced by user interaction behavior rather than the rating value itself: users who engage more with the platform are more likely to leave ratings. Because the missingness in both cases is plausibly driven by observed variables rather than the unobserved missing values, these patterns are consistent with MAR and can be formally evaluated using permutation tests.

### Contributors' Presence & Recipe Descriptions
<u> Null Hypothesis:</u> The missingness of descriptions does not depend on the number of recipes published by authors. 

<u> Alternate Hypothesis:</u> The missingness of descriptions does depend on the number of recipes published by authors.

<u> Test Statistic:</u> Difference in mean number of recipes published between authors whose recipes include descriptions and those whose recipes are missing descriptions.

<u>Significance Level:</u> 0.05

<iframe src="/Figures/Recipe_count_desMissingness.html" width="100%" height="500"></iframe>

A permutation test with 2,000 iterations was conducted to evaluate whether the observed difference between the group with missing descriptions and the group with non-missing descriptions could have arisen by chance.

<iframe src="/Figures/Recipe_count_desMissingness_perm.html" width="100%" height="500"></iframe>


Authors of recipes with missing descriptions published, on average, 418 fewer recipes than authors of recipes with descriptions (<b>observed difference = –418.2 </b>, denoted by the black vertical line). A <b>p-value of 0.0005</b> < 0.05 from the permutation test indicates this difference is highly unlikely to have arisen by chance, rejecting the null hypothesis. These results suggest that description missingness is likely influenced by observed variables rather than the unobserved content itself, making it most likely <b>missing at random (MAR)</b>.


### Calories & Rating 
<u> Null Hypothesis:</u> The missingness in ratings does not depend on the amount of calories in recipes. 

<u> Alternate Hypothesis:</u> The missingness in ratings does depend on the amount of calories in recipes.

<u> Test Statistic:</u> Difference in mean calories between recipes with missing ratings and recipes without missing ratings.

<u>Significance Level:</u> 0.05

<iframe src="/Figures/Cal_ratingMissingness.html" width="100%" height="500"></iframe>

A permutation test with 2,000 iterations was conducted to evaluate whether the observed difference between the group with missing rating and the group with non-missing rating could have arisen by chance.

<iframe src="/Figures/Cal_ratingMissingness_perm.html" width="100%" height="500"></iframe>

Recipes with missing ratings had, on average, 60.67 more calories than recipes with observed ratings (<b>observed difference = 60.67</b>, denoted by the black vertical line). A <b>p-value of 0.0005</b> < 0.05 indicates this difference is very unlikely due to chance, rejecting the null hypothesis. These results suggest that rating missingness is likely influenced by observed variables rather than the unobserved rating value itself, making it most likely <b>MAR</b>.


### Cooking time & Rating 
<u> Null Hypothesis:</u> The missingness in ratings does not depend on the recipes' cooking time. 

<u> Alternate Hypothesis:</u> The missingness in ratings does depend on the recipes' cooking time.

<u> Test Statistic:</u> Difference in mean cooking time between recipes with missing ratings and recipes without missing ratings.

<u>Significance Level:</u> 0.05

<iframe src="/Figures/CookingTime_ratingMissingness.html" width="100%" height="500"></iframe>

A permutation test with 2,000 iterations was conducted to evaluate whether the observed difference between the group with missing rating and the group with non-missing rating could have arisen by chance.

<iframe src="/Figures/CookingTime_ratingMissingness_perm.html" width="100%" height="500"></iframe>

Recipes with missing ratings had, on average, 34.89 more minutes of cooking time than recipes with observed ratings (observed difference = 34.89, denoted by the black vertical line). A <b>p-value of 0.114 > 0.05 fails to reject the null hypothesis</b>, suggesting this difference could plausibly have been by chance. These results indicate that cooking time is not significantly associated with rating missingness.


