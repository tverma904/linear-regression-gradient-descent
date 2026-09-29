# Linear Regression & Gradient Descent

## Overview

This project demonstrates linear regression with one variable and the use of Gradient Descent to optimize the model parameters `w` and `b`.

The experiment uses a small housing-price dataset to demonstrate how a linear model makes predictions and how Gradient Descent improves the model parameters by minimizing the cost function.

## Objectives

- Implement linear regression with one variable.
- Compute predictions using the linear model.
- Calculate the cost function.
- Compute the gradients with respect to `w` and `b`.
- Optimize `w` and `b` using Gradient Descent.
- Compare the actual values with the final model predictions.

## Dataset

The experiment uses the following illustrative training data:

- `x_train = [1.0, 2.0]`
- `y_train = [300.0, 500.0]`

Here, `x` represents house size in 1000 square feet and `y` represents price in thousands of dollars.

Since the dataset contains only two training examples, this project is intended as an educational demonstration of linear regression and Gradient Descent rather than a real-world housing-price prediction system.

## Linear Regression Model

The linear model used in the experiment is:

`f(x) = wx + b`

where:

- `w` is the model parameter (weight).
- `b` is the bias/intercept.
- `x` is the input feature.
- `f(x)` is the predicted value.

## Cost Function

The Mean Squared Error-based cost function is used to measure the difference between the predicted and actual values.

The cost is calculated using the predictions, actual values, and current values of `w` and `b`.

## Gradient Descent

Gradient Descent is used to automatically optimize `w` and `b`.

The experiment starts with:

- `w = 0`
- `b = 0`
- Learning rate `α = 0.01`
- Iterations = `10,000`

At each iteration, the gradients are calculated and the parameters are updated to reduce the cost.

## Implementation

The project implements the following functions from scratch:

- `compute_model_output()` — generates predictions.
- `compute_cost()` — calculates the cost.
- `compute_gradient()` — calculates the gradients.
- `gradient_descent()` — optimizes `w` and `b`.

No `sklearn` linear regression model is used.

## Results and Visualization

The notebook includes visualizations of:

- The original housing-price training data.
- The initial linear model predictions.
- The final linear fit after Gradient Descent.
- Actual versus predicted housing prices.

The final optimized values of `w` and `b` are also displayed along with the model's predictions.

## Technologies Used

- Python
- NumPy
- Matplotlib
- Google Colab

## How to Run

1. Open the notebook in Google Colab or Jupyter Notebook.
2. Run the cells sequentially.
3. Observe the initial model and predictions.
4. Run the Gradient Descent implementation.
5. Review the optimized parameters and final visualization.

## Conclusion

This experiment demonstrates the basic working of linear regression and shows how Gradient Descent can automatically optimize the model parameters `w` and `b` to obtain predictions that fit the given training data.
