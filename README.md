# 21-deep-learning-challenge

## Overview of the analysis: 

### Preprocessing
In the data preprocessing section:
1. read the data 
2. clean the feature data to fewer categories 
3. split the target and feature data to train data and test data
4. scale the feature data 

### Compiling, Training, and Evaluating the Model
In the compiling, training, and evaluating the model section:
1. create a neural network model with three layers
2. complie the model
3. train the model
4. evaluate the model with the data

## Results: Using bulleted lists and images to support your answers, address the following questions:

### Data Preprocessing

What variable(s) are the target(s) for your model?
-The column *IS_SUCCESSFUL* is the target for the model.

What variable(s) are the features for your model?    
-The columns: *APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT* are the features for the model.

What variable(s) should be removed from the input data because they are neither targets nor features?
-The columns: *EIN and NAME* are the identification columns, so they should be removed from the input data.

### Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
- I used three layers. The first layer use 80 units and 43 input dimensions, and relu as the activation function. The second layer I use 30 units and relu as the activation function. The last layer I use 1 unit and sigmoid to get the output. 
- The reasons I choose those functions are that I don't see that the data has a negative part, the output only need to be 0 or 1, and I had tried different functions and neurons amount but got the similar result, therefore, I keep the one that use the less time to run.
![nn_model_summary1](image.jpg)
![nn_model_summary1_1](image.jpg)
![nn_model_summary2](image.jpg)
![nn_model_summary2_1](image.jpg)
![nn_model_summary3](image.jpg)
![nn_model_summary3_1](image.jpg)


Were you able to achieve the target model performance?
-The model performance was lower than I expert since it only has 0.56 as the loss and 0.73 as the accuracy.

What steps did you take in your attempts to increase model performance?
- I tried increase the neurons amount, increase the layers amount, and change the activation function as the pictures above.


## Summary: 
-After prepocessing the data and build the neural network model, I got the model loss 0.56and accuracy 0.73, which is not a very good model. 
-For the models I have learned, I may recommand using the K-Nearest Neighbors model, since it is a good model for predict classification result and it is easy to use. 