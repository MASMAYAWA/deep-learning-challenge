# deep-learning-challenge

1. Overview of the Analysis:
The purpose of this analysis is to predict whether applicants will be successful if funded by Alphabet Soup. This involves utilizing deep learning techniques to build a model that can accurately classify whether funding recipients will effectively utilize the allocated resources.

2. Results:

Data Preprocessing:

Target Variable(s) for Model:
['APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', 'ASK_AMT']

Feature Variable(s) for Model:
'IS_SUCCESSFUL'

Variable(s) Removed from Input Data:
'EIN' and 'NAME'

Compiling, Training, and Evaluating the Model:

Neurons, Layers, and Activation Functions Selected: Initially, the model had 2 hidden layers with 80 neurons in the first layer and 30 neurons in the second layer, using ReLU activation function. However, despite tweaking hyperparameters, accuracy remained at around 0.7286. Subsequently, a method was created to automatically optimize the model. The best model obtained had:  
Activation: 'sigmoid'  
Neurons in the input layer: 57  
Neurons in the hidden layers (6 of): 5, 83, 25, 69, 59, 53  
Tuner parameters: Epochs=7  
This resulted in a marginal improvement in accuracy to 0.7342.  

3. Summary:
The deep learning model's performance, while showing slight improvement through hyperparameter optimization, still falls short of the desired target accuracy (75%). It seems that the complexity of the problem and the nature of the dataset pose challenges for the current modeling techniques.

Recommendation:
Considering the limitations of the deep learning model, it may be beneficial to explore alternative, more sophisticated approaches. 
