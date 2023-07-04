# Kaggle-rider-app-competition

Step-wise Explanation:
*The ‘train’ excel file is imported to spss. As the estimated_ride_duration and estimated_ride_distance showed very 
strong correlation, these two variables cannot be treated as two different variables in regression, nor we can delete 
these because both of the variables are important. So we make a variable named “mixed” in spss, which is the mean of 
these two variables. 
*The COMPLETED status was recoded as 1, and the CANCELED status was recoded as 0. 
*After putting all the variables into independent variables at first in linear regression and deleting stepwise, we finally 
found the model with the highest adjusted R squared and p-values less than 0.05. The dependent variable is 
estimated_fare.
Model:
Y = .021*MIXED + .219*discount_new - 14.136*status + 36.881
(R squared: .849, Adjusted R squared: .848)
*The respondents containing missing values of relevant variables were removed completely. 
*Finally the model is applied to test file using the corresponding variables. 
