# deep_learning_challenge
## Report on the Performance of the Deep Learning Model for Alphabet Soup

### Overview of the Analysis:
The purpose of this analysis is to develop a deep learning model using neural networks to predict whether funding from Alphabet Soup, a charitable organization, will be used effectively by various organizations. The goal is to achieve a target predictive accuracy higher than 75% to aid Alphabet Soup in making informed decisions about funding allocation.

### Results:

### Data Preprocessing:

* Target Variable: The target variable for the model is IS_SUCCESSFUL, which indicates whether the funding was used effectively (1) or not (0).
* Feature Variables: The feature variables for the model include APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.
* Variables to be Removed: The identification columns EIN and NAME should be removed from the input data as they are neither targets nor features.
* For the optimized learning model I added NAME back in as a Feature Variable and I removed STATUS, ORGANIZATION and INCOME_AMT. 


### Compiling, Training, and Evaluating the Model:
Neurons, Layers, and Activation Functions For the Optimized Learning Model:
* Input layer with 19603 neurons (equal to the number of features).
* Five hidden layers with 100, 50, and 10 neurons.
    * Increasing the number of neurons in each layer allows the model to learn more complex patterns in the data, potentially improving its predictive power.
    * Multiple hidden layers were included to enable the model to learn hierarchical representations of the data
* ReLU activation functions for all hidden layers.
* Sigmoid activation function for the output layer.
Achieving Target Model Performance: The model achieved an accuracy above 75% on the training data. When evaluating the model it came out to 76% accurate
Steps to Increase Model Performance: To improve model performance, I experimented with different architectures, including adding more layers and neurons, and adjusting the features. By doing that I was able to increase the accuracy from 72% to 76%


### Summary:
The deep learning model developed for Alphabet Soup's funding prediction achieved moderate performance and consistently met the target accuracy of 75%. To potentially improve model performance, I could 
* Ensemble Learning: Combining multiple models (e.g., different neural network architectures or algorithms) to leverage their collective predictive power.
* Feature Engineering: Creating additional features or transforming existing ones to capture more relevant information for the prediction task.
