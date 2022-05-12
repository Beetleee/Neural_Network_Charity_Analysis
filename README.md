# Module 19 Neural Network Modeling  

### by Terra Lasho 
## Overview of the Analysis: For this project, I have created a deep learning model for AlphabetSoup, using knowledge of machine learning and neural networks.  I used a dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by AlphabetSoup.
-----------------------------------------------------------------------------------------------------------------------------------
## Overview of the Analysis
------------------------------------------------------------------------------------------------------------------------------------
## Deliverable 1: Preprocessing Data for a Neural Network Model
### Part 1: Open the file in pandas dataframe:
![](https://github.com/Beetleee/Credit_Risk_Analysis/blob/main/Resources/Plot1.png)
### Part 2: Drop the EIN and Name Columns in the dataset:
![](https://github.com/Beetleee/Credit_Risk_Analysis/blob/main/Resources/Plot2.png)
### Part 3: Determine the unique datapoints for each column:
![](https://github.com/Beetleee/Credit_Risk_Analysis/blob/main/Resources/Plot3.png)
### Part 4: Density Plot (to create a cut-off point to bin “rare” categorical variables in a new column “other”):
![](https://github.com/Beetleee/Credit_Risk_Analysis/blob/main/Resources/Plot4.png)
### Part 5: Merge the one-hot encoding dataframe with the original and drop the originals:
![](https://github.com/Beetleee/Credit_Risk_Analysis/blob/main/Resources/Plot5.png)
### Part 6: Split the preprocessed data into features and target arrays, and then into training and testing datasets, then standardize numerical variables using StandardScaler:
![](https://github.com/Beetleee/Credit_Risk_Analysis/blob/main/Resources/Plot6.png)
-------------------------------------------------------------------------------------------------------------------------------
## Deliverable 2: Compile, Train, and Evaluate the Model
### Part1: This deep-learning neural network model was initially made of two hidden layers with 30 and 25 neurons respectively.  The input data has 40 features and 25,724 samples. The output is binary classification.
 ![](https://github.com/Beetleee/Credit_Risk_Analysis/blob/main/Resources/Plot7.png)
### Part2: To speed up the training process, we are using “ReLU” as the activation function for the hidden layers, and “Sigmoid” is used on the output layer for our binary classification.  
![](https://github.com/Beetleee/Credit_Risk_Analysis/blob/main/Resources/Plot8.png)
### Part3: For the compilation, the optimizer is “adam” and the loss function is “binary_crossentropy”.
![](https://github.com/Beetleee/Credit_Risk_Analysis/blob/main/Resources/Plot9.png)
### Part4: The model efficiency was under 75%, and is not a satisfying performance.
![](https://github.com/Beetleee/Credit_Risk_Analysis/blob/main/Resources/Plot10.png)
## Deliverable 3: Optimize
### We tried an additional 2 times to optimize the model.  The second time we ran the network, we increased the number of neurons on both of the hidden layers, and added a third hidden layer “ReLU” (AlphabetSoupCharity-Copy1)
![](https://github.com/Beetleee/Credit_Risk_Analysis/blob/main/Resources/Plot11.png)
Unfortunately we did not increase the efficiency:
![](https://github.com/Beetleee/Credit_Risk_Analysis/blob/main/Resources/Plot12.png)
### The last time we ran the network, we increased the number of neurons on the hidden layers (AlphabetSoupCharity-Copy2)
![](https://github.com/Beetleee/Credit_Risk_Analysis/blob/main/Resources/Plot13.png)
Unfortunately we did not increase the efficiency:
![](https://github.com/Beetleee/Credit_Risk_Analysis/blob/main/Resources/Plot14.png)
## Summary
The deep learning neural network model did not reach the target of 75% accuracy. Recommendations would be to utilize a Random Forest Classifier (since we have a binary classification situation). This would combine multiple decision ‘trees’ in order to generate a classified output and test/analyze its performance against our model.
