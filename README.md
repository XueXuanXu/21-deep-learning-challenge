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
2. compile the model
3. train the model
4. evaluate the model with the data

## Results: Using bulleted lists and images to support your answers, address the following questions:

### Data Preprocessing

What variable(s) are the target(s) for your model?   
- The column *IS_SUCCESSFUL* is the target for the model.

What variable(s) are the features for your model?    
- The columns: *APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT* are the features for the model.

What variable(s) should be removed from the input data because they are neither targets nor features?
- The columns: *EIN and NAME* are the identification columns, so they should be removed from the input data.

### Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
- I used three layers. The first layer uses 80 units and 43 input dimensions, and relu as the activation function. In the second layer I use 30 units and relu as the activation function. In the last layer I use 1 unit and sigmoid to get the output. 
- The reasons I chose those functions are that I don't see that the data has a negative part, the output only needs to be 0 or 1, and I had tried different functions and neurons amount but got similar results, therefore, I keep the one that use the less time to run.
![nn_model_summary1](https://github.com/XueXuanXu/21-deep-learning-challenge/blob/main/image/nn_model_summary1.PNG)
![nn_model_summary1_1](https://github.com/XueXuanXu/21-deep-learning-challenge/blob/main/image/nn_model_summary1_1.PNG)
![nn_model_summary2](https://github.com/XueXuanXu/21-deep-learning-challenge/blob/main/image/nn_model_summary2.PNG)
![nn_model_summary2_1](https://github.com/XueXuanXu/21-deep-learning-challenge/blob/main/image/nn_model_summary2_1.PNG)
![nn_model_summary3](https://github.com/XueXuanXu/21-deep-learning-challenge/blob/main/image/nn_model_summary3.PNG)
![nn_model_summary3_1](https://github.com/XueXuanXu/21-deep-learning-challenge/blob/main/image/nn_model_summary3_1.PNG)


Were you able to achieve the target model performance?    
- The model performance was lower than I expected since it only has 0.56 as the loss and 0.73 as the accuracy.

What steps did you take in your attempts to increase model performance?   
- I tried to increase the neurons amount, increase the layers amount, and change the activation function as the pictures above.


## Summary:     
- After preprocessing the data and building the neural network model, I got a model loss of 0.56 and an accuracy of 0.73, which is not a very good model. 
- For the models I have learned, I may recommend using the K-Nearest Neighbors model, since it is a good model for predicting classification results and it is easy to use. 
