# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Hamza Tahiri

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
TODO: Predictions would be rejected if some of the prediction values were less than zero, so all negative prediction values should be set to zero.

### What was the top ranked model that performed?
TODO: WeightedEnsemble_L3

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
TODO: There was no clear distribution. Additional features added by using Pandas' 'dt' feature (dt.year, dt.month, and dt.day) to create new columns from the year, month, and day pieces of the datetime column values.

### How much better did your model preform after adding additional features and why do you think that is?
TODO: Better. Kaggle score decreased from about 1.80042 to 1.34 

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
TODO: The model performed slightly better after trying different hyperparameters

### If you were given more time with this dataset, where do you think you would spend more time?
TODO: Categorizing features as either numerical or categorical data.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|default|default|default|1.31910|
|add_features|default|default|default|0.56439|
|hpo|random|5|light|1.80042|       0042
### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![modrainrain_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png)

## Summary
TOThe performance of an Autogluon model on the bike sharing demand dataset improved after separating the datetime column of the dataset into month, day, and year columns and optimizing the time_limit, num_stack_levels, and num_bag_folds parameters.tion
