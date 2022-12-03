# MechaCar_Statistical_Analysis
Module 16
## Linear Regression to Predict MPG

The linear regression model is -103.964 + 6.27*setwvehicle_length + 0.00*vehicle_weight + 0.07*spoiler_angle + 3.55*ground_clearance + -3.41*AWD. 

In the coefficiencies call out result, it appears there are variables including intercept, setwvehicle_length, ground_clearance impacting mpg due to the significant probability value that each coefficient contributes a random amount of variance. 

With impact of intercept value, it means that there are some other variables affecting mpg that does not include in this model. 
However, since the model p value is less than 0.05 and r squre value is > 0.5, it could mean current variables still represents a positive correlation to mpg.
![image](https://github.com/jilldvn/MechaCar_Statistical_Analysis/blob/main/image/mpg_prediction%20model.png)


## Summary Statistics on Suspension Coils 

Based on customer's specifications, variance of the suspension coils must not exceed 100 pounds per square inch, from the following descriptive findings, considering overall variance is at 67 PSI, it meets the requirement of less than 100 PSI variance.
Individually, both Lot 1 and 2 meets customer's spect with variance less than 100 PSI. Lot 3, however, with PSI variance 170, does not meet customer's specitifcations. 
![image](https://github.com/jilldvn/MechaCar_Statistical_Analysis/blob/main/image/total_summary.png)
![image](https://github.com/jilldvn/MechaCar_Statistical_Analysis/blob/main/image/lot_summary.png)

## T-Tests on Suspension Coils
### Here is a hightlight of wheter or not suspnsion coils average is equal to 1500 PSI in each group:
![image](https://github.com/jilldvn/MechaCar_Statistical_Analysis/blob/main/image/one%20sample%20t-test%20results.png)

1. One Sample t-test on sample population, p-value is 0.06028, greater than alpha risk, failed to reject null hypothesis, as a result we can interprete the mean of PSI on all sample population is equal to 1500.
2. One Sample t-test on Lot 1, p-value is 1, greater than alpha risk, failed to reject null hypothesis which indicates the mean of PSI on Lot 1 is equal to 1500.
3. One Sample t-test on Lot 2, p-value is 0.6072, greater than alpha risk, failed to reject null hypothesis which indicates the mean of PSI on Lot 2 is equal to 1500. 
3. One Sample t-test on Lot 3, p-value is 0.04168, less than alpha risk, reject null hypothesis which means the average of PSI on Lot 3 is not equal to 1500. 


## Study Design: MechaCar vs Competition
More metrics can be analyzed per market requirement. Using current available dataset, one example is to compare with with mpg efficiency with whether or not the vehicle is AWD. 
We may peform a two sample t test with unequal sample size. 

In this case, null hypotheisi is AWD vehicle's average of fuel efficiency (mpg) has no difference from non AWD vehicle (equal mean). In contrast, alternative hypothesis is AWD vehicle's average of fuel efficiency (mpg) is significntly differnt from non AWD vehicle. 
