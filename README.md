# Logistic-Regression
Detailed description and practical application of logistic regression

Goals: Describe how you found the optimum threshold value using accuracy, sensitivity, and specificity. How did you optimize your model? Plot ROC, find the key measures of classification and print the confusion matrix. 
## Logistic Regression:: 
## Logistic regression is a statistical method for binary classification. It predicts the likelihood of an event occurring based on input features, producing a probability between 0 and 1 using the sigmoid function
### It is called "regression" because it has its roots in the broader family of regression models(or the generalization of linear regression). Linear regression fails to predict output only in a certain range and also there occurs a shift in the best-fit line as outliers increase.

The sigmoid function, also known as the logistic function, is a mathematical function that maps any real-valued number to a value between 0 and 1. It's commonly used in logistic regression to model the probability of a binary outcome.

The sigmoid function is defined as:
![image](https://github.com/pavi-1994/Logistic-Regression/assets/81359749/721bf711-e84b-4b6a-920c-a836b5d9edf4)


where:
y or it is also represented as σ(x) is the output or value of the sigmoid function.

e is the base of the natural logarithm (approximately equal to 2.71828).

x is the input to the function.

Originally, it was developed for binary classification problems, where the goal was to predict the probability of a binary outcome. The logistic function (sigmoid function) is used to map the output of the model to a probability. Parameters are optimized using gradient descent to minimize a cost function. The model defines a decision boundary, separating the classes. It's widely used in fields like healthcare and marketing for tasks like disease prediction and customer churn analysis.


### Assumption of logistic regression:
1. Binary Outcome: Logistic regression assumes the dependent variable is binary, meaning it has only two possible outcomes.

2. Linearity in Log Odds: It assumes a linear relationship between the independent variables and the logarithm of the odds.

3. No Multicollinearity: Independent variables should be independent of each other (no multicollinearity).

4. Large Sample Size: It performs well with a large sample size to ensure stable estimates.

5. No Outliers: Outliers can influence the estimation of parameters.

6. Independent Errors: Errors should be independent of each other.

7. No Endogeneity: There should be no correlation between independent variables and the error term.

8. No Homoscedasticity: It does not assume constant variance across levels of the dependent variable.


### Pros and Cons of Logistic Regression

#### 1. Pros of Logistic Regression:

Interpretability: It provides interpretable results, allowing you to understand the impact of each predictor variable on the probability of the outcome.

Efficient with Small Data: It can work well even with relatively small datasets and is less prone to overfitting compared to more complex models.

Fast Training and Prediction: Logistic regression models are computationally efficient, making them quick to train and make predictions.

Probabilistic Output: It directly models the probability of the outcome, making it useful for tasks where understanding the likelihood of an event is important.

#### 1. Cons of Logistic Regression:

Linear Assumption: It assumes a linear relationship between the independent variables and the log of odds of the outcome. It may not perform well if the relationship is highly non-linear.

Limited to Binary Classification: While there are extensions for multi-class classification, logistic regression is primarily designed for binary classification tasks.

Sensitive to Outliers: Outliers can heavily influence the parameter estimates and predictions.

Doesn't Handle Missing Data Well: If the dataset has a significant amount of missing data, logistic regression may not be the best choice without proper handling of missing values.



##### We are using the logistic regression to classify whether Email Spam or Ham: 
About Data: The data contains 4 columns ['Unnamed: 0', 'label', 'text', 'label_num'] and all belong to the 'object' datatype

1. importing data
2. data preprocessing
3. exploratory data analysis
4.  model building

## Conclusion: 
In the case of Spam mail Detection, we will more focus on False Positives. This is so because, In the case of False-Positive the model will predict the unspam mail as spam which results in the loss of some useful data. If the ham mail that was recognized as spam contains any important information, it will not be reached to the user. 
