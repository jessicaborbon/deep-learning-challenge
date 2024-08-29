# Alphabet Soup - Neural Network Model Report

## 1. Overview
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.


## 2. Results
#### Data Preprocessing

a.	What variable(s) are the target(s) for your model?  
•	The target variable is the ‘IS_SUCCESSFUL’ column within application_df with a 1 (yes) and 0 (no)  

.b.	What variable(s) are the features for your model?

There were many features for the first model: 
NAME 19568
APPLICATION_TYPE 17
AFFILIATION 6
CLASSIFICATION 71
USE_CASE 5
ORGANIZATION 4
STATUS 2
INCOME_AMT 9
SPECIAL_CONSIDERATIONS 2
ASK_AMT 8747

.c.  What variable(s) should be removed from the input data because they are neither targets nor features?
The variables that were removed from the input data were the columns ‘EIN’ and ‘NAME’ because neither one of them were targets nor features in the first model.   
#### Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why? 

The first model I had two hidden layers with ten hidden neurons in the first layer and five hidden neurons in the second layer which produced 6781 parameters and epochs were set to 100.
![alt text](<Screenshot/Screenshot 2024-08-29 at 11.27.07 AM.png>)
There were 4320 parameters created by the 2 layers in the training model.
![alt text](<Screenshot/Screenshot 2024-08-29 at 11.29.18 AM.png>)

* Were you able to achieve the target model performance?

No, The first attempt was about 73% accurate but was aiming for at least 75% accuracy.
![alt text](<Screenshot/Screenshot 2024-08-29 at 11.31.19 AM.png>)

* What steps did you take in your attempts to increase model performance?

Using multiple layers helps to train the machine learning model based on filtering the data. Adding the name column into the dataset greatly increased the accuracy of the model.  Classification counts were set to 30 and a third hidden layer was added.  The parameters increased to 14370 and epochs were adjusted to 50.  The layers were adjusted as follows:
![alt text](<Screenshot/Screenshot 2024-08-29 at 11.35.46 AM.png>)
![alt text](<Screenshot/Screenshot 2024-08-29 at 11.38.50 AM.png>)


## 3. Summary
The first model came up short with an accuracy score of 73.21%.  The second optimization model with all the adjustments gave much better accuracy of 78.82% and would be the better model to use for to determine if applicants were successfully funded.
![alt text](<Screenshot/Screenshot 2024-08-29 at 11.43.31 AM.png>)