# Neural_Network_Charity_Analysis

## Overview of the loan prediction risk analysis
Compare differencce between tradition ML and regression models also Neural Network. Describe model and its components. Explain difference in neural network structures that change alorithm. Implementing Neural network by using TensorFlow. 
## Results
- Data Preprocessing
  - What variables are considered the targetes for model ?
    
    The "IS_SUCCESSFUL" column is our target variable. We aim to predict if an application will be accepted and this column represents our desired outcome.
    
  - What variables are considered to be features for your model ?
    
    Features use:
    - APPLICATION_TYPE
    - AFFILIATION
    - CLASSIFICATION
    - USE_CASE
    - ORGANIZATION
    - INCOME_AMT
    - SPEICIAL_CONSIDERATIONS
    
  - What variables are neither targets nor feautres, and should be removed from the input data ?
   
    The 'EIN' and 'Name' variables are not relevant to our analysis.
    
- Compiling, Training, and Evaluating the model
 
  - How many neurons, layers, and activation functinos did you select you for your neural network, and why ?
    
    I chose to use 2 node layers with 80 and 30 neurons. I selected the ReLU activation function for the hidden layers and the sigmoid activation function for the output layer as we are dealing with binary output. The number of epochs was set to 100. I added many neurons to my layers to ensure each neuron could concentrate on a unique feature and to make it easier and quicker to find the optimal weights by having multiple neurons in the layers.
    
    ![Screenshot 2023-02-07 at 00 13 58](https://user-images.githubusercontent.com/112133209/217191912-3b69a100-afe3-4f9f-8f39-948d9b0086db.png)
    
  - Were you able to achieve the target model performance ?
    
    With the target accuracy ~ 73% i was barely able to achieve the performace
    
    ![Screenshot 2023-02-07 at 00 24 46](https://user-images.githubusercontent.com/112133209/217191963-0a7a2f7e-b74b-4997-a650-68b9f09845c4.png)

  - What steps did you take to try to increase model performance ?
    
    Well after adding third hidden layer the accuracy has dropped to about 57%. So i would just use 2 hidden layer and up to 100 epoch would be worked fine. 
## Summary
Efforts to improve the original model were mostly unsuccessful. Despite trying various parameters of the deep learning model, the best accuracy achieved was 72.7%, which falls short of the goal of 75% accuracy. Given that the model's output is binary classification, it may be better to consider using a supervised machine learning approach such as a random forest classifier.
