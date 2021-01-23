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

<p float="left">
  <img src="https://user-images.githubusercontent.com/67468718/105615300-65ce0980-5d84-11eb-8915-1a500a2482ac.JPG" width="750" />
  <img src="https://user-images.githubusercontent.com/67468718/105615299-65357300-5d84-11eb-9ede-eee198be9cb6.JPG" width="350" /> 
</p>
