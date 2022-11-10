# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

Vehicle length and ground clearance are the two 2  variables that provide a non-random amount of variance to the mpg values in the dataset. As shown in the above, screen shot, these independent variables' coefficients are extremely close to 0. Additionally, they have a significant relationship between each other and the dependent variable, mpg.

The slope of the linear model is not considered to be 0. This is demonstrated in the p-value since it is significantly smaller than the alpha value. The p value is 5.35e-11 and the alpha value (significance value) is 0.05. 

The linear model does not predict the mpg of MechaCar prototypes extremely effectively, but it does an adequate job. This is demonstrated by the R-squared value. The R-squared value is 0.7149, which means that approximately 71.49% of the variability of the dependent variable (mpg) is explained using this linear model.  

![linear_regression_summary](https://user-images.githubusercontent.com/109561408/200986980-5ae1b3f2-bf07-4e6d-9cbc-e6535c4c4cbb.png)

## Summary Statistics on Suspension Coils

In total, the variance of the suspension coils is 62.29. This shows that the total variance does meet the current manufacturing specification. When analyzing each lot individually, it is shown that both lots 1 and 2 have relatively low variances: 0.98 and 7.47, respectively. Lot 3 has a variance of 170.28. Lots 1 and 2 individually meet the current manufacturing specification, but Lot 3 does not. 

![image](https://user-images.githubusercontent.com/109561408/200987046-4e17187b-f7ec-43b7-951d-e84632ff9486.png)

![image](https://user-images.githubusercontent.com/109561408/200987100-b3ee6e47-5e87-43fa-be67-47b560e1186d.png)

## T-Tests on Suspension Coils

For the t-tests, it was determined determined that the null hypothesis is mu = 1500. The alternative hypothesis is mu not = 1500. 

The Lot 1 t-test displays a p-value of 0.06. Since this value is greater than our alpha value of 0.05, we fail to reject the null hypothesis. This means that we cannot definitively say that the mean PSI is not equal to 1500. 

![image](https://user-images.githubusercontent.com/109561408/200987281-076a9f0c-3dc9-4278-aa6b-a0e9e97415bb.png)

Similarly, the Lot 2 t-test displays a p-value greater than the alpha value. The alpha value is always 0.05 in this analysis. The p-value for Lot 2 is 0.61, which means that we fail to reject the null hypothesis. We cannot definitively say that the mean PSI for Lot 2 is not equal to 1500.

![image](https://user-images.githubusercontent.com/109561408/200987333-865a0f82-444e-4504-bff8-9429e53449dd.png)

The Lot 3 t-test calculates a p-value of 0.04, which is lower than the alpha value of 0.05. Because of this, we reject the null hypothesis. Additionally, the t-test in R displays a confidence interval, which in Lot 3 is 1492.43 to 1499.85. Since 1500 does not lie between these values and the p-value is lower than the alpha value, we can definitely say that the mean PSI is not equal to 1500. 

![image](https://user-images.githubusercontent.com/109561408/200987377-f6647830-679e-4fab-9d72-51399aed7b1b.png)

## Study Design: MechaCar vs Competition
