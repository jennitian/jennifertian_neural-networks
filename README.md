# Neural Networks
module 19 challenge
## Goals
To create a deep neural network learning model to predict the success of various charitable organizations to better allocate resources for donations.

## Analysis
For this project, I used tensor flow to create a neural network to predict success of various charities. In processing the dataset, I first removed name id columns and then identified categorical variables in the dataframe. From there I looked at the number of unique categories in each column and reduced the number of unique values to <= 10 for the necessary columns. After this, I could use OneHotEncoder to translate each category to a numerical value for analysis by the program. After scaling the existing numerical columns, the dataset was ready for analysis. I chose a neural network containing 3 hidden layers for this analysis because there are 10 input columns after cleaning the data and we need 1 output. I found that increasing the number of hidden layers improved our accuracy for the analysis. As for the number of neurons in each layer, I follwed to 2-3 x rule and started the first layer at 30 neurons and gradually halved the number of neurons with each layer to narrow down our results. The final accuracy of the model measured around 73%, with a 55% loss metric. 
