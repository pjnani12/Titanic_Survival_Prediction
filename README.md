# Titanic_Survival_Prediction
To predict the Survival of a person from Titanic Data-Set using Decision Tree Algorithm.

## Algorithm: Decision Tree

The motive of using Decision Tree is to create a training model which can use to predict class or value of target variables by learning decision rules inferred from training data.
The Decision Tree Algorithm tries to solve the problem, by using tree representation. Each internal node of the tree corresponds to an attribute, and each leaf node corresponds to a class label.
The primary challenge in the decision tree implementation is to identify which attributes do we need to consider as the root node and each level.

The popular attribute selection measures:

i)Gini Index:
To measure how often a randomly chosen element would be incorrectly identified. It means an attribute with lower gini index should be preferred.

ii)Entropy:
Measure of the randomness in the information being processed.            
lower the entropy -> higher the information gain.

APPROACH:
1.	gathered dataset from kaggle
https://www.kaggle.com/c/titanic/data
2.	Pre-processing
Handling Missing Values
LabelEncoder: 
The categorical values have been converted into numeric values,
encode labels with a value between 0 and n_classes-1 where n is the number of distinct labels. If a label repeats it assigns the same value to as assigned earlier.
Removed Outliers
3.	split dataset in features and target(label) variable
4.	Random split of training Data-set in 70:30 rating for training and testing
5.	Creating Decision Tree model and training the model
6.	Testing (Predict the response for test dataset)
7.	Calculating the accuracy for the output
8.	With the results, built confusion matrix, Precision, Recall, F_Score
9.	Plotted ROC curve and Decision Tree.


RESULTS: 
Using entropy we got accuracy of 76.9%

Precision :  0.657
Recall    :  0.675
F_Score   :  0.666

Suggestion for Improving the model:

Finding more optimized parameters for the decision tree classifier by searching over the parameter space can improve the model.
Achieved Accuracy after improvement: 0.783410138248848
