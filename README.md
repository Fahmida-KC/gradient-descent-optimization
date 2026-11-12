# Gradient Descent Optimization Algorithms

## Project Overview

This project implements three gradient descent optimization algorithms from scratch using Python and NumPy for linear regression. The objective is to understand and examine how different gradient update strategies optimize model parameters by minimizing a Mean Squared Error (MSE)-based cost function.

## Algorithms Implemented

- **Batch Gradient Descent (BGD):** Computes gradients using the entire training dataset before updating model parameters.
- **Mini-Batch Gradient Descent (MBGD):** Divides the dataset into smaller batches and updates parameters after each mini-batch.
- **Stochastic Gradient Descent (SGD):** Updates model parameters individually for each training observation.

## Methodology

The linear regression hypothesis function was defined as `h_theta(x) = theta_0 + theta_1 * x`.

The implementation involved:

1. Creating synthetic datasets for linear regression.
2. Initializing model parameters and learning rates.
3. Calculating predictions and errors.
4. Computing gradients with respect to the intercept and slope.
5. Iteratively updating parameters using the three optimization algorithms.
6. Monitoring cost changes and final parameter estimates over 1,000 epochs.

## Experimental Configuration

| Parameter     |          BGD |  MBGD |   SGD |
| ------------- | -----------: | ----: | ----: |
| Dataset size  |            3 |    10 |    10 |
| Learning rate |          0.1 |  0.01 |  0.01 |
| Batch size    | Full dataset |     4 |     1 |
| Epochs        |        1,000 | 1,000 | 1,000 |

## Results

Final estimated model parameters:

| Algorithm                   | Intercept (θ₀) | Slope (θ₁) |
| --------------------------- | -------------: | ---------: |
| Batch Gradient Descent      |         1.0000 |     2.0000 |
| Mini-Batch Gradient Descent |         0.6644 |     1.5136 |
| Stochastic Gradient Descent |         0.6669 |     1.5336 |

The experiments illustrate the differences in parameter update mechanisms and cost behavior across the three gradient descent approaches.

*Note: Different synthetic datasets were used for BGD and for MBGD/SGD. Therefore, the numerical results are not a controlled performance comparison.*

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

## Repository Structure

```text
gradient-descent-optimization/
│
├── gradient_descent.ipynb
└── README.md
```

## Key Learning Outcomes

- Understanding the mathematical foundations of gradient descent.
- Implementing gradient calculations and parameter updates from scratch.
- Exploring the effects of batch size on optimization.
- Examining convergence behavior and cost fluctuations.
- Applying iterative optimization to linear regression.
