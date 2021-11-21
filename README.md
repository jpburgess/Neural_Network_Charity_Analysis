# Neural_Network_Charity_Analysis

## Overview

The purpose of this analysis was to train a neural network to classify if organizations that used Alphabet Soup will effectively use the money they raised.

## Results
### Data Preprocessing
- The "IS_SUCCESSFUL" feature was used as the target
- The features were: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
- EIN and NAME were removed from the features list

## Compiling, Training, and Evaluating the Model
### Model Structure:
- Hidden Layer 1: 50 nodes, Relu activation
- Hidden Layer 2: 30 nodes, Relu activation
- Output Layer: 1 node, Sigmoid activation

### Model Performance
- The model was able to reach 68.7% accuracy

### Optimization
- The first attempt used the provided model of (80 nodes, relu), (30 nodes, relu), (1 node, sigmoid)
- This had 53% accuracy and the loss went to zero which suggested overfitting to me
- The second attempt reduced the number of nodes in the first layer to 50 and decreased the epochs to 50 and changed the optimizer to adamax
- This had an accuracy of 68%
- The final attempt reduced the nodes from 50,30 to 40,10
- This had an accuracy of 56%

## Summary
With more time spent optimizing the model and looking into removing/cleaning the features this model could have a much higer accuracy.  A different model such as a support vector machine would work well for this problem. SVM's work well for binary classifaction problems such as this.  
