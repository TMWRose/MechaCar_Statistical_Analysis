# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
![model summary](https://user-images.githubusercontent.com/100237685/183472292-e3215cc8-605e-4da1-994b-9bcd48a54554.png)


1. **Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?**
- The AWD, vehicle_weight, and spoiler_angle provided an non-random amount of variance.

2. **Is the slope of the linear model considered to be zero? Why or why not?**
- The slope is not considered to be zero because we rejected the null hypothesis as our p-value was less than 0.05. 

3. **Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?**
- If the limited variables provided are all the company is looking for to predict the mpg of the prototypes then yes, the model predicts it effectively at ~71.5% success rate. There are other elements that can affect the mpg of a car, so the company might want to consider expanding the number of variables. 





## Summary Statistics on Suspension Coils
![total summary](https://user-images.githubusercontent.com/100237685/183479889-5298a5f9-c354-4670-87b7-3798e7da7ce7.png)
![lot summary](https://user-images.githubusercontent.com/100237685/183479922-eef35c16-68fb-4a8d-bb5d-003f8f375b8f.png)

1. **The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?**
- The current manufacturing data *does not* meet the design specifications for *all* lots as they all have wildly different variance values. 
- Lot 1 have a variance of ~0.98, making it the most consistent and reliable
- Lot 2 has a variance of ~7.47, which isn't terrible but there will be some discrepancy
- Lot 3 has a variance of ~170.29, which is way above the allowed variance levels




## T-Tests on Suspension Coils


### All Lots
![t test all lots](https://user-images.githubusercontent.com/100237685/183484254-9f917583-ad8c-43d4-b062-2a8b0785efdc.png)

- Since p-value > 0.05, we accept the null hypothesis which means there is  no statistical difference between the observed sample mean and its presumed population mean.
- However, as seen by the t-value and the mean of x, the all lots sample mean is lower than the population mean, indicating that all lots together have a higher variance from the population data. 



### Lot 1
![t test lot 1](https://user-images.githubusercontent.com/100237685/183484311-4bfeafb9-8d12-452e-9e8a-d4d3897c6e1a.png)

- Since p-value > 0.05, we accept the null hypothesis which means there is no statistical difference between the observed sample mean and its presumed population mean.
- In this instance, the t-value = 0 and the mean of x is exactly equal to the population mean, indicating that Lot 1 has the least amount of variance from the population data.


### Lot 2
![t test lot 2](https://user-images.githubusercontent.com/100237685/183484369-5f012035-b8b6-4e64-9b6f-a114e9b8c90e.png)

- Since p-value > 0.05, we accept the null hypothesis which means there is no statistical difference between the observed sample mean and its presumed population mean.
- The t-value in this case is positive, indicating the mean of this sample is slightly higher than the population mean (which is confirmed by looking at mean of x). There is some variance in this sample from the population but not enough to be signifigant.


### Lot 3
![t test lot 3](https://user-images.githubusercontent.com/100237685/183484411-2922fafd-edcb-4362-a1d0-2b6a600d892b.png)

- For Lot 3 p-value < 0.05, which means we **reject** the null hypothesis and there *is* a statistical difference between the observed sample mean and its presumed population mean.
- This sample has the most variance of them all from the population data.
- However, while on its own the variance is enough to statistically differentiate it, when added to the all plots sample set, it does not make a signifigant enough difference to affect the all plots p-value towards rejecting the null hypothesis. 



## Study Design: MechaCar vs Competition

*Write a short description of a statistical study that can quantify how the MechaCar performs against the competition. In your study design, think critically about what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating.*

1. **What metric or metrics are you going to test?**
- In addition to the metrics mentioned in the instructions, I would also add mpg, AWD, color options, intiror material, Bluetooth compatibility, bonus features (such as seat warmers, sunroofs, etc.), and dashboard technology (whether it's touch screen, big or small, etc.).
2. **What is the null hypothesis or alternative hypothesis?**
- H0 = consumer expecations are met
- Ha = consumer expectations are either not met or exceeded
3. **What statistical test would you use to test the hypothesis? And why?**
- I would use a Two Sample t-Test because I would be testing each metric from MechaCar and the competitor company individualy against a consumer sentatmeint score for each metric to see if there is a differecne in the mean. If there is a signifigant difference, then you can check the varience and t-value to see if the difference is leaning towards a positive or negative sentament from the consumer. 
- For example, if we know that consumers like between 10-15 color options, we can run a two -sample t-test with the number of color options from MechaCar (sample 1) and the number of color options from competitor comapny (sample 2). Depending on the p-value and the t-value, we'll be able to tell if there is a signifigant difference from the population (consumer) mean, and if there isn't that means the company meets consumer expectations, but if there is a difference we'd need to look at the t-value to see if it is negative or postive, which will tell us if the company exceeds or falls short of consumer expectations. 
4. **What data is needed to run the statistical test?**
- We would need sentatmint analysis from a consumer study for each of our variables
- We would also need the data on each of the varibles from both MechaCar and any competitors they want to compare themsleves to. 


