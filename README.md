# Overview
In this project, we generated 1000 random input numbers, created 9 additonal features based on the randomly generated numbers, reduced their dimensionality using PCA, trained 2 linear regression models, using the original inputs and PCA-generated components, and created plots to compare the predictions.

# Inference
In this particular case, we can see that only 2 PCA components were sufficient to capture 95% of the variance in the 10 input features.
Using the plots, we can see that the  predicitons using the PCA components are in-line with the predictions made by the original input features.

# Process

1. Generate 1000 random numbers between 0 and 10.
2. Create a dataframe with 10 columns, where each column = random_data raised to the power of it's column position, i.e
   - column 1 = random_number**1
   - column 2 = random_number**2
   - column 3 = rodom_numner**3
   .
   .
   - column 10 = random_number**10
3. Generate a target variable y, which is the sum of all of the input features.
4. Split the data into train and validation data.
5. Generate PCA componenets of the train data.
6. Model 1 - Train a Linear Regression model using the original input features.
7. Model 2 - Train a Linear Regression model using the PCA components.
8. Make predictions for validation data using Model 1 (original input features).
9. Make predictions for validation data using Model 2 (PCA generated features).
10. Plot the predicitons made by Model 1 and Model 2 against the validation target.

