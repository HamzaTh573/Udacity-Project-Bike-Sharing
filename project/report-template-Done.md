# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Hamza Tahiri

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
When attempting to submit predictions, it was discovered that negative prediction values would lead to rejection. To address this, all negative prediction values were adjusted to zero.

### What was the top ranked model that performed?
The top-ranked model that performed was the WeightedEnsemble_L3.

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
During exploratory analysis, no clear distribution patterns were discerned. Additional features were created by leveraging Pandas' 'dt' feature, extracting year, month, and day components from the datetime column values.

### How much better did your model preform after adding additional features and why do you think that is?
After incorporating additional features, the model's performance significantly improved. The Kaggle score decreased from about 1.3191 to 0.56439, indicating enhanced predictive accuracy.

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
While experimenting with different hyperparameters, the model exhibited slight performance improvements.

### If you were given more time with this dataset, where do you think you would spend more time?
Given additional time, more attention would be dedicated to categorizing features as either numerical or categorical data.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|------------|-------|-------|-------|-------|
|initial     |default|default|default|1.31910|
|add_features|default|default|default|0.56439|
|hpo         |random |5      |light  |1.80042|      

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![modrainrain_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png)

## Summary
The performance of the AutoGluon model on the bike sharing demand dataset significantly improved after incorporating additional features extracted from the datetime column and optimizing specific hyperparameters. This resulted in a notable decrease in the Kaggle score, indicating enhanced predictive accuracy.
