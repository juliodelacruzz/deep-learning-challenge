# deep-learning-challenge
Module 21 Challenge UCB Data Analyst Bootcamp 2024


**OVERVIEW**
The purpose of this challenge was to create a machine learning algorithm that would help accurately predict whether or not an applicant would be successful if funded by Alphabet Soup. From there, we need to make any necessary adjustments to the model so we can reach an agreeable accuracy score of 75%.


**RESULTS**
Data Preprocessing
The target would be if the applicant is successful.
This means that all the other columns would be our features.
![targetANDfeature](https://github.com/juliodelacruzz/deep-learning-challenge/assets/31105353/d65c6a0d-3c43-45cc-ba5b-05e83e54aefd)

However, before we do this, we must drop any unnecessary columns from our dataset that will not provide value to our machine model. We must drop columns 'EIN' and 'Name' because these columns are neither targets or features. They are just ID's for the applicants, which have no value for our model.
![droppedColumns](https://github.com/juliodelacruzz/deep-learning-challenge/assets/31105353/7ea9b529-2f40-43e0-a451-c5fb91dc3af4)

Compiling, Training, and Evaluating the Model
Originally, there were two layers. The first layer had 80 nodes and the second had 30. The activation functions that were used was relu for the hidden layers and sigmoid for the output layer.
Using these, the original accuracy of the model was 0.7295 or 72.95%. This was also ran with 100 epochs.
![originalMODEL](https://github.com/juliodelacruzz/deep-learning-challenge/assets/31105353/b90d201c-29d2-448f-acd8-8899ac456ed9)
![ogACC](https://github.com/juliodelacruzz/deep-learning-challenge/assets/31105353/a21a2d60-a6ff-411a-8ff7-f4eb955ae0f3)

For the first optimization attempt, I tried adding another layer of 15 nodes with the same activation. I also used the same amount of epochs. However this had no apparent change in the accuracy as I got around 72% again.
![optimized1](https://github.com/juliodelacruzz/deep-learning-challenge/assets/31105353/b709caf6-fb3a-4eab-aaea-0dd85641be42)
![1optimizedACC](https://github.com/juliodelacruzz/deep-learning-challenge/assets/31105353/111b7bd0-38a6-47d2-a1a1-ca14b46adf87)

For the second optimization attempt, I switched up the activation to leaky relu. Running the same amount of epochs, this improved my accuracy to 73.15%. 
![optimized2](https://github.com/juliodelacruzz/deep-learning-challenge/assets/31105353/87949c22-a1d3-4d35-b140-fbe9af140f9d)
![2optimizedACC](https://github.com/juliodelacruzz/deep-learning-challenge/assets/31105353/87590f2c-2afc-4678-8bcb-635a23693d36)


For the third attempt, I tried adding a fourth layer and increased the epochs to 150. This was not able to increase my accuracy. The accuracy obtained was 72.86%
![optimized3](https://github.com/juliodelacruzz/deep-learning-challenge/assets/31105353/32e9c2cb-9c83-45a6-aa5a-14042c0bc1b2)
![3optimizedACC](https://github.com/juliodelacruzz/deep-learning-challenge/assets/31105353/5d74d782-1121-4b50-95aa-ae4f25f1d800)


**SUMMARY**
I was not able to get the targeted 75% accuracy, althought I was able to get quite close when I used leaky relu. I think in the future I would explore more activation methods and look for any other type of classification models that may be a better fit for this dataset. I know that in previous classes there were methods to find the best number of layers and neurons for a data set. I would reccommend using those types of methods as I think they would positvely affect the accuracy score.
