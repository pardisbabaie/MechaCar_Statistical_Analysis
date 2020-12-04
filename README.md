# MechaCar_Statistical_Analysis
## Linear Regression to Predict MPG
Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
- The two variables that provided a non-random amount of variance to the mpg values and should be considered are vehicle length and ground clearance as they are statistically significant as shown in the data below.

Is the slope of the linear model considered to be zero? Why or why not?
- To determine if the slope of the linear model is considered to be zero, we would test the following hypothesis for linear regression:
  - H0 : The slope of the linear model is zero, or m = 0
  - Ha : The slope of the linear model is not zero, or m ≠ 0
- Based on this since there is a significant statistical relationship with vehicle length and ground clearance and our p-Value 5.35e-11 is significantly smaller than the significance level of 0.05%, we can conclude that the there is significant evidence to reject out null hypothesis and that the slope of the linear model is not considered to be 0.

Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
- From the linear regression model shown below, the r-squared value is 0.71, which portrays that approximately 71% of the relationship between the prototype dimensions and MPG will be correct using this model. As 71% is above 50%, this model does effectively explain the relationship between the protoype diminsions and MPG. However, this is just based on two statistically significant values so the linear model is not ideal and we need more significant variables. 

<img width="512" alt="Screen Shot 2020-12-03 at 6 48 24 PM" src="https://user-images.githubusercontent.com/69806770/101106075-480ed000-359d-11eb-92a1-bc14c58d8889.png">

## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
- As shown below the overall variance of all manufacturing lots in total is 62.3 which is less than 100 pounds so it does meet this design specification.

<img width="321" alt="Screen Shot 2020-12-03 at 7 34 41 PM" src="https://user-images.githubusercontent.com/69806770/101107128-a341c200-359f-11eb-9ee1-1ed1d7c25d83.png">

- As shown below the variance of lot 1 which is 0.98 and lot 2 which is 7.47 are both below 100 pounds and meet the design specification. However, the viariance of lot 3 is 170.29 which is significantly higher than the design specification of not exceeding 100 and fail this design specification.

<img width="490" alt="Screen Shot 2020-12-03 at 7 34 31 PM" src="https://user-images.githubusercontent.com/69806770/101107154-b2c10b00-359f-11eb-9325-ff3224277bc0.png">

## T-Tests on Suspension Coils
As shown below in the t.test of Lot 1 we can see the p-value is 1.568e-11 which is much less than 0.05 so we can say with a 95 percent confidence interval that the means are statistically significantly different.

<img width="634" alt="Screen Shot 2020-12-03 at 7 57 23 PM" src="https://user-images.githubusercontent.com/69806770/101108579-d76ab200-35a2-11eb-97e7-ac2e38a58d8f.png">

As shown below in the t.test of Lot 2 we can see the p-value is 0.0005911 which is much less than 0.05 so we can say with a 95 percent confidence interval that the means are statistically significantly different.

<img width="628" alt="Screen Shot 2020-12-03 at 7 57 34 PM" src="https://user-images.githubusercontent.com/69806770/101108606-ea7d8200-35a2-11eb-97cb-684ce4e4289f.png">

As shown below in the t.test of Lot 3 we can see the p-value is 0.1589 which is greater than 0.05 so we can say with a 95 percent confidence interval that the means are not statistically significantly different.

<img width="630" alt="Screen Shot 2020-12-03 at 7 57 49 PM" src="https://user-images.githubusercontent.com/69806770/101108846-6972ba80-35a3-11eb-890b-6f61822183b4.png">

## Study Design: MechaCar vs Competition
In this study, to determine how MechaCar is performing against the competition we are going to look at a few metrics to be tested: cost, safety rating and horse power. The null hypothesis is:
- H0 : MechaCar does no perform better than the competition in any of the metrics tested.

The statistical test I would use for this is a one-way ANOVA for each variable/metric. This way we can test the cost, safety rating and horse power of the MechaCar against the same metric for multiple competitors and see how we perform against multiple competitors.By seeing how we perform against competitors in each of these metrics we can rank ourselves against the competition and make a decision in which metrics we are able to improve to out perform the competition.
To run these tests, we need the information of cost, safety rating and horse power for MechaCar as well as the same data from our competitors so that we can test this data against each other. This is public information for car competitors so should be easily accessible. The data type should be interval as we should capture this data for a specific timeframe i.e. past 6 months to capture the most relevant data for our current circumstances and decision.

