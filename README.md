# Neural Network Charity 

# Overview of the analysis

## The purpose of this Challenge was to use deep-learning neural networks along with the TensorFlow software library in order to perform an analysis and classify which organizations were the most successful from the charitable donations. 

# First Steps

 PreProcess the data in order to get ready for the neural network model (NNM),
 Then trained and evaluated the model,
 Finally made 3 attempts to optimize the model

# Results

### PreProcessing Steps

 The primary focus was on Column IS_SUCCESSFUL as the target for the model
 The columns APPLICATION_TYPE, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT were the features of the model
 The columns EIN and NAME were not targets or features, so they were removed from the input data.

### Compiling, Training, and Evaluating

The neural network model created had two hidden layers. The first layer had 80 neurons and the second layer had 30. The output layer is made up of a unique neuron because it holds a binary classification. The first and second hidden layers had the "relu" activation function, the output layer contained the "sigmoid" activation function. We did not achieve a targeted accuracy score of 75%; the accuracy score for this model was aprroximately 72.54%. For the optimazation stage we made 3 attempts to try and improve the accuracy score. The 1st attempt we removed the 'AFFILIATION' column. This did not improve the accuracy which hovered around 72.16%. For the 2nd attempt we increased the number of neurons on one of the hidden layers and used a model with three hidden layers. We also tried leveraging a different activation function called (tanh) but this also did not help to improve the model's performance.

# Summary
The Neural Network model utilized did not reach an accuracy score of 75% even after three different attempts to optimize the model. It is evident that the model is not outperforming. The recommendation would be to consider the other Supervised machine learning models such as the Random Forest Classifier, or Support Vector Machine in order to combine a higher number of decision trees which will generate a classified output and then we will be able to evaluate its performance score versus this deep learning model. 