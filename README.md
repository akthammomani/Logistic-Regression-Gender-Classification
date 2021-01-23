# Project: Gender Classification using Logistic Regression

### Predict the person gender based on their weight and height using Logistic regression model

![Logistic_reg](https://user-images.githubusercontent.com/67468718/105578429-0d235000-5d35-11eb-9afa-505d657abfd8.JPG)

## 1. Introduction: 

**Logistic regression** is a *supervised learning classification algorithm* used to predict the probability of a target variable. The nature of target or dependent variable is dichotomous, which means there would be only two possible classes.
Mathematically, a logistic regression model predicts P(Y=1) as a function of X. It is one of the simplest ML algorithms that can be used for various classification problems such as spam detection, Diabetes prediction, cancer detection etc.
Here , we use the Logistic regression model to predict the gender(Male/Female) of the person based on their weight and height .
The data set contains three columns
  * Height in inches
  * Weight in pounds
  * Gender (Male/Female) of the person
  
## 2. Visualization & Feature Engineering:   

Let's explore the correlations and see which features separate the Male\Femals populations:

Pairplot per Gender         |  Correlation
:-------------------------:|:-------------------------:
![Pairplot](https://user-images.githubusercontent.com/67468718/105615300-65ce0980-5d84-11eb-8915-1a500a2482ac.JPG) | ![corr](https://user-images.githubusercontent.com/67468718/105615299-65357300-5d84-11eb-9ede-eee198be9cb6.JPG)

<p align="center">
  <img width="800" height="500" src="https://user-images.githubusercontent.com/67468718/105615301-65ce0980-5d84-11eb-8369-bfc3c5ad0320.JPG">
</p>

## 2. Tuning Logistic Regression (hyperparameter Tuning): 

The model has some hyperparameters we can tune for hopefully better performance. For tuning the parameters of our model, we will use a mix of **cross-validation** and **grid search**. In Logistic Regression, the most important parameter to tune is the **regularization parameter** **C**. Note that the regularization parameter is not always part of the logistic regression model. 

**regularization parameter** **C** is used to control for unlikely high regression coefficients, and in other cases can be used when data is sparse, as a method of feature selection.

#### Let's use 2 methods to perform model tuning and selecting the regularization parameter **C**:
  1. Writing our own loops to iterate over the model parameters
  2. Using **GridSearchCV** to find the best model
  
## 3. Training vs Validation:

After completing above steps we have conculded that the best **regularization parameter** **C**: 1  correspondes to the max validation score: 0.9172

<p align="center">
  <img width="800" height="500" src="https://user-images.githubusercontent.com/67468718/105616033-b9425680-5d88-11eb-9d46-3a1c56b79048.JPG">
</p>

  


