# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Jason Chau

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
I needed to set non-negative values for Kaggle to accept.

### What was the top ranked model that performed?
My top ranked model is WeightedEnsemble_L3.

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
In EDA, I found that datetime was not able to plot in a histogram. For the same reasons, modle training was not able to interpret some month and year data.

### How much better did your model preform after adding additional features and why do you think that is?
The Kaggle score received is substantially more than previous (x2).

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
My model was no better after hyperparameter tuning.

### If you were given more time with this dataset, where do you think you would spend more time?
I would spend more time finding more features.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|time_limit|num_bag_folds|keep_only_best|score|
|--|--|--|--|--|
|initial|600|10|False|1.39101|
|add_features|600|10|False|4.76188|
|hpo|1200|15|False|4.76188|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

![model_train_score.png](model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

![model_test_score.png](model_test_score.png)

## Summary
In train plot, I notice that hyperparameter tuning is scoring less than the prvious model. This is probably overfitting. I noticed that new features is greatly improving given scores. I will first consider feature engineering for future ML projects.
