# logistic-regression-from-scratch
📄 Project Documentation: Logistic Regression via Perceptron Trick & Sklearn Comparison
Title: Logistic Regression: Manual Implementation with Perceptron Trick vs. Sklearn
Author's Objective:
To explore how Logistic Regression can be understood from scratch using the Perceptron learning rule, and compare the results with the sklearn implementation.

🧠 Core Concepts and Flow
1. Logistic Regression Background
Purpose: Draw a linear boundary (decision line) between two classes.

Equation: 
𝐴𝑥1+𝐵𝑥2+𝐶=0
Classes: Positive class (1) and Negative class (0)

🔧 Implementation Details
✅ Data Generation:
100 2D points using make_classification from sklearn.
Linearly separable data with clear separation between classes.
✅ Initial Line Assumption:
Start with a random line: 
𝑥1+𝑥2-1=0

Visualized using Matplotlib.

✅ Perceptron Trick (Manual Implementation):
Introduces a step function to predict class.

Weights updated using:

new_weights =old_weights+𝛼(𝑦_actual−𝑦_pred)⋅𝑋

Simple rule for binary classification, similar to Perceptron logic.

Plotted the updated decision line based on final weights.

✅ Drawback Noted:
Hard step function leads to non-differentiable updates.

Not ideal for logistic regression, which should use sigmoid activation and log loss.

📊 Comparison with Sklearn Implementation
Trained logistic regression model from sklearn.linear_model.LogisticRegression

Compared coefficients and intercept with manual perceptron implementation.

Plotted both decision boundaries:

Black line: Perceptron trick

Red line: Sklearn logistic regression

✅ Bonus: Sigmoid-Based Manual Update
Attempts a second manual implementation using sigmoid activation in the step function.

Compared all three boundaries:

Perceptron trick

Sklearn logistic regression

Perceptron + Sigmoid (Logistic regression inspired)
