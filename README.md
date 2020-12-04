# MechaCar_Statistical_Analysis
## Linear Regression to Predict MPG
- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
The two variables that provided a non-random amount of variance to the mpg values and should be considered are vehicle length and ground clearance as they are statistically significant as shown in the data below.
- Is the slope of the linear model considered to be zero? Why or why not?
To determine if the slope of the linear model is considered to be zero, we would test the following hypothesis for linear regression:
  - H0 : The slope of the linear model is zero, or m = 0
  - Ha : The slope of the linear model is not zero, or m ≠ 0
Based on this since there is a significant statistical relationship with vehicle length and ground clearance and our p-Value 5.35e-11 is significantly smaller than the significance level of 0.05%, we can conclude that the there is significant evidence to reject out null hypothesis and that the slope of the linear model is not considered to be 0.
- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
From the linear regression model shown below, the r-squared value is 0.71, which portrays that approximately 71% of the relationship between the prototype dimensions and MPG will be correct using this model. As 71% is above 50%, this model does effectively explain the relationship between the protoype diminsions and MPG. However, this is just based on two statistically significant values so the linear model is not ideal and we need more significant variables. 

<img width="512" alt="Screen Shot 2020-12-03 at 6 48 24 PM" src="https://user-images.githubusercontent.com/69806770/101106075-480ed000-359d-11eb-92a1-bc14c58d8889.png">

## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
- As shown below the overall variance of all manufacturing lots in total is 62.3 which is less than 100 pounds so it does meet this design specification.

<img width="321" alt="Screen Shot 2020-12-03 at 7 34 41 PM" src="https://user-images.githubusercontent.com/69806770/101107128-a341c200-359f-11eb-9ee1-1ed1d7c25d83.png">

- As shown below the variance of lot 1 which is 0.98 and lot 2 which is 7.47 are both below 100 pounds and meet the design specification. However, the viariance of lot 3 is 170.29 which is significantly higher than the design specification of not exceeding 100 and fail this design specification.

<img width="490" alt="Screen Shot 2020-12-03 at 7 34 31 PM" src="https://user-images.githubusercontent.com/69806770/101107154-b2c10b00-359f-11eb-9325-ff3224277bc0.png">
