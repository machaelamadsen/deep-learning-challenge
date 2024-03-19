# Deep Learning Challenge Report
## Overview
In this analysis I created a binary classifier to help Alphabet Soup determine if applicants for funding will be successful if funded. This was done with the use of machine learning and neural networks. The data was first preprocessed. Then the model was compiled, trained, and evaluated. From here I worked to optimize the model.

## Results

# Data Preprocessing

* Target Variables: The target variable is the 'IS_SUCCESSFUL' column.
* Feature Variables: The feature variables are all comuns besides the target variable, and the previously dropped columns('EIN' and 'NAME')
* Variables to be removed because they are neither targets nor features: The removed variables are EIN and NAME.

# Compiling, Training, and Evaluating the Model

* 6 Neurons in the first layer and 8 in the second were originally selected. I did this as a starting point to see what my accuracy results were then increased them to 8 and 10 respectively to attempt to improve accuracy by helping the neural network learn more complex patterns.
* 3 layers were used per the assignment. The first two used relu activation functions. Relu introduces nonlinearity and avoids vanishing gardient. I used sigmoid for the output layer. This is best used in models where the probability has to be predicted and there is only the range of 0 to 1.
* I was not able to achieve the target model performance. I got accuracy to reach 73%
* In my attempts to increase model performance I increased the number of nodes in each layer, decreased the batch size, raised then decreased the cutoff values, and dropped the 'USE_CASE' column


## Summary
Overall the model was able to reach 73% accuracy with 55% loss. It is a good model, but has room for improvement and can't be completely trusted. I would recommend using random forest as an improvement. This can improve accuracy with reduced risk of overfitting and help determine feature importance. By removing less important features from the model accuracy may be increased.
