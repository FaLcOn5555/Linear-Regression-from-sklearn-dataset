# Linear-Regression-from-sklearn-dataset
## 📖 Project Description
This project demonstrates how linear regression models—including Linear Regression, Ridge Regression, and Lasso Regression—can be used to predict house prices using the Boston Housing dataset. The aim was to understand model behavior, compare performances, and apply regularization techniques to avoid overfitting.

## Methodology
### Data Loading & Exploration:
The Boston Housing dataset was loaded using Scikit-learn. Basic exploratory data analysis was performed to understand feature distributions and their correlation with the target variable (house price).

### Feature-Target Separation:
The dataset was split into independent features (e.g., RM, LSTAT, CRIM) and the dependent target variable (Price) for modeling.

## Linear Regression Model:
A simple linear regression model was trained using 5-fold cross-validation. The model achieved a mean negative mean squared error (MSE) of approximately -34.70, which indicates a reasonable baseline performance.

### Ridge Regression (L2 Regularization):
<br>
Ridge regression was implemented with a range of alpha values using GridSearchCV to find the best penalty term.<br>
🔹 Best alpha value: 20 <br>
🔹 Best MSE: -34.07 <br>
This shows that applying L2 regularization helped reduce overfitting and slightly improved performance. <br> 

### Lasso Regression (L1 Regularization):
Lasso regression was also tested with a similar hyperparameter tuning approach. <br>
🔹 Best alpha value: 1 <br>
🔹 Best MSE: -34.46 <br><br>
While Lasso didn’t outperform Ridge, it provides the added benefit of feature selection by shrinking less relevant coefficients to zero.
