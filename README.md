# Neural Network Model Report

## Analysis Overview
The purpose of this analysis is to create an algorithm using machine learning in order to predict whether applicants for funding through Alphabet Soup will be success or not. 

## Results: 

### Data Preprocessing

1. What variable(s) are the target(s) for your model?
- The target variable is the 'IS_SUCCESSFUL' column from application_df
2. What variable(s) are the features for your model?
- The feature variables are every other column from application_df --> this was defined by dropping the 'IS_SUCCESSFUL' column from the original dataframe
3. What variable(s) should be removed from the input data because they are neither targets nor features?
- The variables 'EIN' and 'NAME' columns were both removed since neither columns were targets nor features for the dataset.

### Compiling, Training, and Evaluating the Model

1. How many neurons, layers, and activation functions did you select for your neural network model, and why?
- In the first attempt, I used 80 in hidden_nodes_layer1 and 30 in hidden_nodes_layer2. These numbers were randomly selected with the understanding that they will be modified to achieve the desired accuracy results later on in the project.
2. Were you able to achieve the target model performance?
- No, I was not able to. The initial run resulted with a 72.93% accuracy.
3. What steps did you take in your attempts to increase model performance?
- In order to increase the model performance, I first dropped the organization and special_considerations column since I doubted whether they were significant to the overall model performance, and then I modified the cutoff values from 500 to 900 to see if that would have any impact. In the next couple attempts, 
I began to modify the two hidden layers to see if there were any changes in result.

## Summary:
Overall, the deep learning model was around 72.2% accurate in predicting the classification problem. Using a model with greater correlation between input and output would likely result in higher prediction accuracy. 
This could be achieved by doing additional data cleanup during the preprocessing stage, perhaps also using a model with different activation functions and iterating again until a higher accuracy is achieved.
