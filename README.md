# Effectiveness-of-FB-ads

Logistic Regression Model¶
Target variable = 'success'. Test-Train-Split my model with 80% training data and 20% testing data at a random state of 35.

Using Sklearn, I ran a baseline Logistic Regression model to examine the Accuracy and F1 score of my engineered features:

Test Accuracy score: 0.5131578947368421

Test F1 score: 0.6782608695652175

The result was not great. The predictive power of my baseline is ~51%, almost the same as flipping a coin.

Feature Selection
I proceeded to use PolynomialFeatures in Sklearn to find all possible interaction terms and polynomials terms (to a degree of 3) and ran my Logistics Regression Model with 35,989 features. Scaling the data using StandardScaler, I arrive at the following results:

Test Accuracy score: 0.9780701754385965

Test F1 score: 0.9785407725321887

In the process of running this model, most of my coefficients went to 0 except for 4,385 features.

Creating a Confusion Matrix, I examined only 2 false negatives and 3 false positives:
