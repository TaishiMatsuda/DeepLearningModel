# DeepLearningModel
Module 19 of UofT Data Analytics Boot Camp

## Overview
Applying machine learning and neural network model to create a binary classifier that is capable of predicting whether or not an applicant will be successful if funded by Alphabet Soup.

#### Resources
* Software / Services: Jupyter Lab
* Programming Language: Python
* Data: Alphabet Soup Charity dataset (Resources/charity_data.csv)

## Methods
1. Pre-processing (Cleanup, Binning, Converting Categorical Variable into Dummy Variables and Scaling).
2. Compiling Neural network model using Tensorflow Keras module. 
3. Optimizing Model by;
    1. Increasing Neurons in Hidden Layer
    2. Increasing Number of Hidden Layer
    3. Using Different Activation Function for Hidden Layer
    4. Increasing Epochs
    5. Preprocessing Data different way
    
## Results
The first model was created using 2 hidden layers with 1st hidden layer consists of 8 neurons and 2nd hidden layer consists of 4 neurons. 2 hidden layers with relatively large number of neurons were selected as the input data had relatively large number of input (57 columns).

The 1st model showed the accuracy of 72.43%.

The results after the optimization shown above is summarized below. Decresing the noise in the input data by binning "APPLICATIONTYPE" in addition to "CLASSIFICATION" increased the accuracy most. However, unfortunately the target of the 75% was not met.

![Results](ResultsByModel.png)

## Other Solution
I would also consider using Random Forest Classifier (RFC) instead of Deep Learning Model. RFC showed the accuracy of 71% which is very close to that of Neural Network Model created above and RFC has significantly less computational cost.