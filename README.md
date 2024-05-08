# deep-learning-challenge
Module 21 Challenge UCB Data Analyst Bootcamp 2024


##**OVERVIEW**
The purpose of this challenge was to create a machine learning algorithm that would help accurately predict whether or not an applicant would be successful if funded by Alphabet Soup. From there, we need to make any necessary adjustments to the model so we can reach an agreeable accuracy score of 75%.


###**RESULTS**
####Data Preprocessing
The target would be if the applicant is successful.
This means that all the other columns would be our features.
![Alt text](images\targetANDfeature.png)

However, before we do this, we must drop any unnecessary columns from our dataset that will not provide value to our machine model. We must drop columns 'EIN' and 'Name' because these columns are neither targets or features. They are just ID's for the applicants, which have no value for our model.
![Alt text](images\droppedColumns.png)

#####Compiling, Training, and Evaluating the Model
Originally, there were two layers. The first layer had 80 nodes and the second had 30. The activation functions that were used was relu for the hidden layers and sigmoid for the output layer.
Using these, the original accuracy of the model was 0.7295 or 72.95%. This was also ran with 100 epochs.

