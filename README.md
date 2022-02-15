![NN](Resources/NN_banner.png)
# Neural Network Charity Analysis

## Overview of the Analysis
The goal of this deep learning analysis was to create a binary classifer that is capable of predicting whether applicants will be successful given the funding. 

The following methods were used for the analysis:
- Preprocessing the data for the neural network model
- Compiling, training and evaluating the model
- Optimizing the model for at least a 75% accurancy

## Resources
- Data Source: [charity_data.csv](https://github.com/nhafer88/Neural_Network_Charity_Analysis/blob/main/Resources/charity_data.csv) from 
- Software: Python, Jupyter Notebook 
## Results
### Data Preprocessing
1. What variable(s) are considered the target for your model?
    - The target for the model is the "Is-Successful" column, stating that the money was effectively used.

2. What variable(s) are considered to be the features for your model?
    - The features are  NAME (taken out later in the analysis for model optimization), APPLICATION, TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT,SPECIAL_CONSIDERATIONS, STATUS, and ASK_AMT

3. What variable(s) are neither and should be removed from the input data? 
    - EIN (Employer identificaiton) was dropped because the column data could lead to confusion and increased error within the machine learning model.
### Compiling, Training, and Evaluating the Model
1. How many neurons, layers, and and activation functions did you select for your neural network model, and why?
    - There are three hidden layers each with many neurons,  because this seemed to increased the accuracy above 75%. 
    - The first activation function was Relu followed by the 2nd and 3rd activation functions being Sigmoid to improve the accuracy. Sigmoid functions and their combinations generally work better in the case of classifiers.

2. Were you able to achieve the target model performance?
    - Target model performance achieved after optimizing model

3. What steps did you take to try and increase model performance?
    - Improving model performance required keeping and converting the NAME column into data points, adding a third layer, and using the Sigmoid activation function for the 2nd and 3rd layer.

## Summary

- By optimizing the model, the accuracy was able to be above 75% for correctly classifying and predicting predicting whether applicants will be successful if funded.
- Further analysis should look at other models, such as RandomForests due to the output being classified.