# Logistic-Regression

This example project demonstrates how Gradient Descent Algorithm may be used to solve Logistic Regression problem as Opposed to solving it by Scikitlearn. Secondly, this project also shows how regularized gradient descent can be used to model non-linear data. 

## Description-

#### Gradient Descent-
Gradient descent is a first-order iterative optimization algorithm for finding the minimum of a function. To find a local minimum of a function using gradient descent, one takes steps proportional to the negative of the gradient (or approximate gradient) of the function at the current point.
Update Equations-
The objective of logistic regression is to minimize the cost function 

![Cost](https://github.com/mustafashabbir10/Logistic-Regression/blob/master/Images/Cost.PNG)

where hypothesis is given by the logistic model-

![Hypothesis](https://github.com/mustafashabbir10/Logistic-Regression/blob/master/Images/hypothesis.PNG)

and the function g is-

![sigmoid](https://github.com/mustafashabbir10/Logistic-Regression/blob/master/Images/sigmoid.PNG)

The parameter of the model are theta values. These are the values I will adjust to minimize the cost function. The most common way to do it is by batch gradient descent. In batch gradient descent, each iteration performs the update

![Iteration](https://github.com/mustafashabbir10/Logistic-Regression/blob/master/Images/Iteration.PNG)

With each step of gradient descent, the parameters thets come close to the optimal values that will achieve the lowest cost.

#### Regulaization-
When the data is not linearly separable then regularized version of gradient descent is used which fits a non-linear classification boundary to the data. The regularized cost function is-
![Regularized_Cost](https://github.com/mustafashabbir10/Logistic-Regression/blob/master/Images/Regularized_cost_func.PNG)

The equation of gradient of gradient descent is-
![Gradient_reg](https://github.com/mustafashabbir10/Logistic-Regression/blob/master/Images/gradient_pd1.PNG)

Here, \lambda is the regularization parameter.
If \lambda equals 0 then no regularization
if \lambda equals 100 high regularization 


### Output-
I have used SciPy to optimize the gradient descent algorithm. Optimize function automatically selects the best learning rate at which the cost will converge and gives us the final output parameters.

![Fit1](https://github.com/mustafashabbir10/Logistic-Regression/blob/master/Images/Logisticfit1.PNG)
The graph above shows the Logistic regression line fitted from Gradient Descent.

#### Regularization-
The graph below shows Logistic Regression fitted for non-linearly separable data using regularization.
![Fit2](https://github.com/mustafashabbir10/Logistic-Regression/blob/master/Images/Logisticfit2.PNG)