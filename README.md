# Multiple Linear Regression with Z-Score Normalization

This project demonstrates the implementation of multiple linear regression to predict house prices using Z-score normalization to improve the performance and convergence of gradient descent.

## Overview

In multi-feature linear regression, features often have vastly different scales (e.g., square footage vs. number of bedrooms). This can cause gradient descent to oscillate or take a long time to converge. Z-score normalization transforms the features so they have a mean of 0 and a standard deviation of 1, resulting in a more symmetric cost function and faster optimization.

## Features

- **Data Loading:** Loads house data including size, number of bedrooms, number of floors, and age.
- **Z-Score Normalization:** Custom implementation of feature scaling.
- **Gradient Descent:** Optimization of weights ($w$) and bias ($b$) using the normalized features.
- **Visualization:** 
    - Scatter plots of features before and after normalization.
    - Comparison of target prices vs. predicted prices.
    - Cost function history.

## Project Structure

- `main.py`: Main script to run the normalization, training, and visualization.
- `lab_utils_multi.py`: Utility functions for data loading and gradient descent.
- `lab_utils_common.py`: Common utility functions and constants.
- `data/houses.txt`: Dataset containing house features and prices.
- `deeplearning.mplstyle`: Custom Matplotlib style for plots.
- `requirements.txt`: Python dependencies.

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd Multiple_Linear_Regression_with_Z-Score_Normalization
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

Run the main script to see the normalization process and the resulting model predictions:

```bash
python main.py
```

The script will:
1. Load the data.
2. Display plots showing the distribution of features before and after normalization.
3. Run gradient descent to find the optimal parameters.
4. Show a final plot comparing the model's predictions with the actual target prices.

## Dependencies

- NumPy
- Matplotlib
- SciPy
