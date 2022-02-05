<p align = "center">
  <img width = "1000" src= "https://user-images.githubusercontent.com/88597956/152655001-67716cfa-4643-42d7-9686-4ab7445cc77d.png">
</p>

## Overview
Using the Alphabet Soup Charity data set, I created a binary classifier that is capable of predicting if applicants will be successful if their charity is funded by Alphabet Soup. This wea done using machine learning and neural networks. 

## Results

### Data Preprocessing
1. What variable(s) are considered the target(s) for your model?
    -  In this data set the target variable used was the IS_SUCCESSFUL column

2. What variable(s) are considered to be the features for your model?
    - APPLICATION_TYPE
    - AFFILIATION
    - CLASSIFICATION
    - USE_CASE
    - ORGANIZATION
    - INCOME_AMT
    - SPECIAL_CONSIDERATIONS
    
3. What variable(s) are neither targets nor features, and should be removed from the input data?
    - EIN and Name were determined to not have any direct correlation in determining if the model would be successful or not. Therefore, the columns were removed from the dataset.

### Compiling, Training and Evaluating the Model
1. How many neurons, layers, and activation functions did you select for your neural network model?
     - As shown below this model has 2 hidden layers. The first layer has 80 neurons and the second layer had 30. Each layer used "relu" as the activation function.
     
        ![Initial_model](https://user-images.githubusercontent.com/88597956/152655890-ed298ec1-3c5c-4551-b378-4cff0da9480c.png)


2. Were you able to achieve the target model performance?
    - The target for the model was 75%. I was able to get relatively close, coming up with an accuracy of 72.6%.

      ![accuracy](https://user-images.githubusercontent.com/88597956/152656010-a85dc474-7b19-4aaa-a2c1-82039afbddd6.png)


3. What steps did you take to try and increase model performance?
    - In an effort to improve the performance of the model, I made 3 changes below to the initial mode and re-ran the model after each change to see if the accuracy increase.
      1. Increased the hidden layers from 2-3
      2. Increased the neurons for each layer from 80, 30, 10 to 100, 60, 20
      3. Changed the activation from relu to tahn
    
    - My accuracy went from 72.6% to 72.5% with the first change. With the second change it further decreased to 72.4% and with the third change it went to back to 72.5% 

## Summary
Overall, I was unable to acheive an accuracy score of 75% with the initial model and the 3 updates to the model. Though we weren't too far off. To improve this model we could use the random forest model as this may prevent in possible overfitting. 
