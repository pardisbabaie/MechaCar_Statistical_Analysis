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

