# **Final Project Pre-Analysis Plan**
*By Ryan Ermovick, Carissa Chen, Iliana Vasslides, Yuthi Madireddy, Kayla Kim*
1. What is an observation in your study?
This study observes one specific instance of a crime. The features consist of year, region, offender race, and offender age, with victim race as a predictor variable. With these, we’ll be observing if a specific race will continue to proportionally be a target/increase/decrease in the future. NOTE: We’re going to add social context from Census data and current event databases to connect to social issues in the modern day.

2. Are you doing supervised or unsupervised learning? Classification or regression?
We are doing supervised learning because the model will be labeled. We will be classifying because our outcome is categorical. There will most likely be a decision tree used for a categorical variable like victim race.

3. What models or algorithms do you plan to use in your analysis? How?
The model that we plan to use to predict the race of the victim is a Decision Tree. We will structure the decision tree around multiple variables, including the region of the attack, year of the attack, age of the offender, and race of the offender. The tree will then be trained on these values and be able to make predictions based on new inputs.

4. How will you know if your approach "works"? What does success mean?
Since we are doing supervised learning, there will be a final result of the victims' race. We can use this to see how accurate the victim race predictions are versus the actual race of the victim. Success means that the variables chosen are influential in determining the category of victims.

5. What are the weaknesses that you anticipate being an issue? How will you deal with them if they come up? If your approach fails, what might you learn from this unfortunate outcome?
While we included several variables, there’s not necessarily a correlation between them and the predictor variable. In addition, many factors influence the results that aren’t included and can’t be adequately quantified or incorporated into a dataset to be analyzed. There are always so many possibilities. While there may be a correlation, none of it can be established as a causation without further analysis. While we can’t directly deal with the problem in the data, we can understand the context of the time because it ends in 2023, so we have additional knowledge of trends over time to predict and make data-driven conclusions based on the results and considering the future.

6. How will you prepare the data specifically for your analysis? For example, are there many variables that should be one-hot encoded? Do you have many correlated numeric variables for which PCA might be a useful tool?
We can prepare the data specifically for our analysis by checking for any missing values we didn’t take care of during the first run-through. We are planning on one-hot encoding at least two variables: Weapon, and Homicide. We are planning on using PCA to compare any correlated numeric variables and based on the variance factors, we can drop off features that do not significantly contribute to the overall cumulative variance. We have to determine if our numeric variables - Victim Sex, Victim Age, Offender Sex, Offender Age, and Year - are correlated using correlation matrices and heatmaps.

7. How will you communicate or present your results? This might be a table of regression coefficients, a confusion matrix, or comparisons of metrics like $R^2$ and RMSE, or accuracy and sensitivity/specificity. This is how you illustrate why your plan succeeded or explain why it failed.
We can analyze the specificity/sensitivity within the prediction. With this, we can take a look at whether the model predicts false positives, true positives (is asian, and predicts is asian), false negatives, and true negatives (is not asian, and predicts is not asian). If there is a significant amount of false positives/negatives compared to the true positives/negatives (more false than true, proportionally distinct in terms of proportion false-proportion true is > .3), then we’ll be able to see if we’ve failed, and can look into why. We can also see if we should add more variables to the decision tree.
	
Possible Extension:
After doing our initial analysis, we hope to perform a smaller, related study of this data. We would like to look at if the murder case was solved or not based off of the prior predictor variables. By looking at if the murder case was solved or not, we might be able to see if the murders of certain races have a higher or lower importance in the police system (assuming that all amounts of evidence are the same because the data for that is not available). 
