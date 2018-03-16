# Regression-Analysis

A lasso regression analysis was conducted to identify a subset of variables from a pool of 20 categorical and quantitative predictor variables that best predicted a quantitative response variable measuring self-esteem of an adolescent. Categorical predictors included  5 binary categorical variables for race and ethnicity (Hispanic, White, Black, Native American and Asian) to improve interpretability of the selected model with fewer predictors. Binary substance use variables were measured with individual questions about whether the adolescent had ever used alcohol, marijuana, cocaine or inhalants. Additional categorical variables included the availability of cigarettes in the home, whether or not either parent was on public assistance and any experience with being expelled from school. Quantitative predictor variables include age, alcohol problems, and a measure of deviance that included such behaviors as vandalism, other property damage, lying, stealing, running away, driving without permission, selling drugs, and skipping school. Another scale for violence, one for depression, and others measuring  parental presence, parental activities, family connectedness and grade point average were also included. All predictor variables were standardized to have a mean of zero and a standard deviation of one.

the data was randomly split into training (70% of the observations) and test dataset (30% of the observations).
The least angle regression algorithm with k=10 fold cross validation was used to estimate the lasso regression model in the training set, and the model was validated using the test set.
The change in the cross validation average (mean) squared error at each step was used to identify the best subset of predictor variables

![2w](https://user-images.githubusercontent.com/18068773/37523605-c25b1240-2927-11e8-84e2-adf1a9f3c13c.png)

This plot shows the change in the mean squared error while the change in the penalty parameter at each step of the selection process
It decreases rapidly at first and then stabilize at point where adding more predictors to the model wouldn’t decrease the mean squared error.


