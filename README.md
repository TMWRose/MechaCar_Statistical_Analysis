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

-
-



### Lot 1
![t test lot 1](https://user-images.githubusercontent.com/100237685/183484311-4bfeafb9-8d12-452e-9e8a-d4d3897c6e1a.png)

-
-


### Lot 2
![t test lot 2](https://user-images.githubusercontent.com/100237685/183484369-5f012035-b8b6-4e64-9b6f-a114e9b8c90e.png)

-
-


### Lot 3
![t test lot 3](https://user-images.githubusercontent.com/100237685/183484411-2922fafd-edcb-4362-a1d0-2b6a600d892b.png)

-
-

