# Neural Network Charity Analysis

## Background
Alphabet Soup is a business making decisions about where to make investments, specifically in applicants for funding.  A model to predict which applicants will be successful is needed for investment decision-making.

### Purpose
Utilizing machine learning and neural networks, a dataset was used to a create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Analysis

### Results

Data Preprocessing:
-	One primary variable was identified for the model, IS_SUCCESSFUL, as being the independent variable.
-	In the initial model all other variables except EIN, NAME, and, IS_SUCCESSFUL were utilized as features.  
-	At minimum EIN and NAME were identified as neither targets or features and removed from the model.  SPECIAL_CONSIDERATIONS and STATUS may not be targets either along with a few other variables; however, that could not be confirmed in the optimization process.

Compiling, Training, and Evaluating the Model:
-	The initial model performed under 70% accuracy; therefore, the number of neurons in layer 1 were increased to 100 and a third sigmoid layer was added with 10 neurons.  Activation function was relu for the first layer and the output layer was sigmoid.
-	To achieve optimization an additional layer was added, the bin sizes changed, and the activation functions changed in the model; however, it was not successful in increasing accuracy of the model.



![Optimized model](https://user-images.githubusercontent.com/80165223/126900660-a082e7f8-d96b-4c4b-b540-a7002c7ba0eb.png)



## Summary

Overall accuracy achieved for both the initial and optimized models was around 69% and, therefore, optimization was not achieved.  This current model cannot assist Alphabet Soup in predicting which applicants will be successful with funding.

A random forest model may be better for this analysis due to dataset size, nonlinear nature of the dataset, and number of input variables.  
