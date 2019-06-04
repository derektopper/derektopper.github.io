---
layout: blog_post
title: Effects of Positional Features on NBA Shot Efficiency
category: blog
---

In this project, I oversaw a team of SAGB members to evaluate what positional features have the highest correlation with made and missed shots.

During this project, I both aided and guided the team’s research through my role as President of the Sports Analytics Group at Berkeley. Below is a description from the paper, [which is available in full here.](https://drive.google.com/file/d/13nbJnjclCQ0HKW-3VD10pADbWEWQgG3P/view?usp=drivesdk)

### Explanation

This project presents a shot classifier for the NBA trained on positional player data and player ratings data to classify individual shot attempts into a make or a miss. 

The classifier has an accuracy of 56.23% on test data, and the precision, recall, and f1­score of our classifier was 0.54, 0.56, and 0.51 respectively. We also present a shot evaluator as an extension of this classifier that outputs a value, 0 to 1, corresponding to the efficiency of a shot. The evaluator was created using a combination of the probability values of our classifier and the type of field goal attempt. 

However, the chief question this paper attempts to answer is what positional features correlate with made and missed shots. The relative strength of features, in terms of predicting made or missed shots, are summarized below. 

Our final model is a logistic regression model that uses positional features in combination with a heuristic based on the player’s shooting ability. The positional features were extracted from game positional data. We proceeded with a logistic regression model in particular as it works well in practice when there are multiple features being used to make a classification decision. 

Interpretability is a key component to our research and the question we are attempting to answer. A novel aspect to our research is that it extends the classification model to create a shot evaluator that can be used to predict what features correlate with a quality shot. This shot evaluator provides great value to teams trying to eliminate inefficiencies in the types of shots they take. After analyzing various features’ effects on the shot evaluator’s score, we concluded that distance from shooter to the basket had the highest correlation with a shot going in or not, and understandably so. 

One surprising result we also noticed is that distance to the nearest teammate had the second largest impact on the shot evaluator’s score. This seems to imply that spacing is very important, especially in the modern NBA. We believe that our research can have a significant impact on modern teams as it demonstrates a way to quantify the efficiency of a shot based solely on positional data, which all NBA teams now have access to. Our hope is that this analysis can be used by NBA coaching staffs to design efficient offenses. 

### Results

After creating this model and analyzing its components and accuracy, we found that although our features were not very strongly correlated with shot efficiency, there was a clear ranking of relative importance between features. 

Most important, by a substantial margin, was distance from the shooter to the basket, which is an understandable result, given that, barring any other factors, shooting percentage is higher the closer one goes to the basket. Distance between the shooter and closest teammate also has an important role, which highlights the role of spacing in today’s offense. 



Features whose coefficients had lesser magnitudes signifying lower importance include ratio of bench players to starters on the floor and number of offensive players outside the three point arc. 

The overall test accuracy of our classifier was 56.23%, suggesting an upper limit to what can be determined by time­-of-shot factors, alone. 

### Future Work

This suggests potential avenues for future work that takes into account possession-­related factors like number of passes or off­-ball movement into the model or even training on individual players. 

Furthermore, analysis can be done on the defensive side of the ball, to see how shot and possession based factors concentrated around defensive efforts impact the result of a shot. Still, the fact that we were able to have some success classifying shots based solely on player position data shows that player tracking data appears to have the potential to refine today’s NBA offenses. 

Moreover, introducing an evaluator that can be used to quantitatively compare different shot attempts and allow a team to optimize for maximal value gives teams clear directions on what they can do with the large collection of data every game provides them.

### Closing Thoughts

This project was a good opportunity for our research team to get our feet wet with NBA positional features. Although our shot evaluator was not perfect, due to the granularity of data available, we certainly had respectable outcomes. The project had interesting results, which seem to make sense. This certainly was a good starting point. 
