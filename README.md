# Neural Network Charity Analysis
## Overview
The purpose of this analysis was to utilize deep learning to help our client, Alphabet Soup, predict whether applicants will be successful in getting funded by them. 

## Results
The results were as follows:

### Data Preprocessing
* The variable that was considered as the target for this model was the "IS_SUCCESSFUL" column.
* The feature variables were all the other columns that weren't the "IS_SUCCESSFUL" column.
* The variables that were neither target nor features were the "EIN" and "NAME" columns as they had no affect on the outcome of the machine learning process. 

### Compiling, Training, and Evaluating the Model
* There were two hidden layers of 80 and 30 neurons, respectively. The activation function for the first and second layer was "relu" in order to speed up the training process, with the activation function for the output layer being "sigmoid". 

![image](https://user-images.githubusercontent.com/86032451/140669352-f6b4dd08-d10c-47d0-b467-6c2f755c055c.png)

* The model was unable to reach the desired accuracy threshold of 75%

![image](https://user-images.githubusercontent.com/86032451/140669447-90425993-f4a4-4ec1-b2fe-bddd13ee5da8.png)

* To help increase the performance of the machine learning model, bucketing was applied to the "ASK_AMT" feature, and the values were then organized by intervals.

![image](https://user-images.githubusercontent.com/86032451/140669604-0bb4e8d1-9a1f-42e4-a305-090fabb28a80.png)

* Another method to help increase the performance was to increase the number of neurons in one of the hidden layers. We also attempted using a model with three hidden layers. 

![image](https://user-images.githubusercontent.com/86032451/140669648-967cd00e-0f75-4ec3-a162-452ee345dbbc.png)
![image](https://user-images.githubusercontent.com/86032451/140669660-b7a29745-4827-4521-b884-0df97996db07.png)

* However, after all the above was attempted the model's performance did not improve:

![image](https://user-images.githubusercontent.com/86032451/140669751-70b61879-dc1b-4c57-a701-29d8f3261c9e.png)

## Summary
In conclusion, we were unable to create a deep learning model that achieved a target accuracy threshold of 75%. Another machine learning that we could attempt, however, would be to use supervised machine learning, such as the Random Forest Classifier, which would allow for us to create a classified output from multiple decision trees, and then compare those results against our deep learning model. 
