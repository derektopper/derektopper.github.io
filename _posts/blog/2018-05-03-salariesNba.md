---
layout: blog_post
title: Classification of NBA Salaries through Player Stats
category: blog
---

In this project, I helped a team of SAGB members to classify the expected salary that a player would recieve in free agency.

During this project, I helped the team better consider the problem and directed certain research threads through my role as President of the Sports Analytics Group at Berkeley. Below is a description from the paper, [which is available in full here.](https://drive.google.com/open?id=1oFumB-YDE51C3CEuzz9yTh_meNbsICIe)

### Basics

This research creates a classification-based model that predicts the salary amounts given to NBA players in free agency. 

In a landscape where obtaining high-value contracts is critical in the success of a franchise, the rise of advanced analytics has enabled more accurate empirical valuations of players. 

This research was done through collecting player salary data through Spotrac and player statistics through Basketball Reference. Correlation analysis demonstrated that points, turnovers, VORP, and rebounds created a balanced and effective set of variables for unweighted KNN-classification. The former three statistics were standardized by year, while the latter statistic was standardized by year and position due to underlying relationships between those categories. 

After classification, the model revealed that volume statistics were most indicative of salaries within lower and mid-level players, while high VORP was common among all players making near-max to max salaries. 

Using test set data, the model was off by 1.21 clusters on average, but many outliers were due to gross over and undervaluation on the part of the franchises. The model was used to predict salaries for incoming free agents in the 2018 class, with reasonable projections that meet qualitative expectations. 

Our model has proven to be a robust predictor of player value from both an empirical and observational standpoint.

Further research is still necessary to prevent the model from overvaluing high volume, “empty stats” players - an issue that GMs still struggle with today. 

In analyzing the results that of our model, we came to the conclusion that our model values high volume scorers over more efficient role players. There is a consistent correlation between PPG, DRB and TOV and predicted salary throughout the entire NBA pay scale. 

While the adage that sports are not played on spreadsheets certainly holds true, and the “eye-test” is still a key component of evaluating players, advanced analytics using machine learning is the next step in more accurately determining a player’s exact value. 

### Closing Thoughts

This project allowed some of our club members to work on a interesting idea with publicly available data. While it is certainly not as black and white as just classifying players based on their top-line stats, this type of method allowed our undergraduate members and opportunity to work with this type of data. The project had interesting results, which seem to make sense. This also certainly was a good starting point for future work with first-party data. 
