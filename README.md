# Neural_Network_Charity_Analysis

## Project Overview

From Alphabet Soup’s business team, we have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

- EIN and NAME—Identification columns
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special consideration for application
- ASK_AMT—Funding amount requested
- IS_SUCCESSFUL—Was the money used effectively

Our task was to perform ETL process on this data then train and test it to create predictions using neural networks on which charities are suceesfull. The accuracy was measured to see how succesful the prediction was.

## Results

- Data Preprocessing
  - What variable(s) are considered the target(s) for your model? **'IS_SUCCESSFUL' column**
  - What variable(s) are considered to be the features for your model? **'APPLICATION_TYPE', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT',      'SPECIAL_CONSIDERATIONS', and 'ASK_AMT'**
  - What variable(s) are neither targets nor features, and should be removed from the input data? **'EIN' and 'NAME'**
  
  
- Compiling, Training, and Evaluating the Model
  - How many neurons, layers, and activation functions did you select for your neural network model, and why? I selected two hidden layers with the following neurons for each   layer. In my optimazation model i played around to achieve higher accuracy.
 **hidden_nodes_layer1 =  24.
   hidden_nodes_layer2 = 12**
  - Were you able to achieve the target model performance? Not at first but with few changes and optimizing the model i was able to achieve close to 75% accuracy
  - What steps did you take to try and increase model performance? I took following steps to increase model performance
    Attempt 1 adding more hidden layers
    Attempt 2 adding neurons
    Attempt 3 Change Activation Function with Callback

## Summary

The deep learning model has a better accuracy score compared to the other models. But comparing between increasing hidden layers vs increasing neurons or epochs, the accuracy was better when we changed activation function with Callback. 
