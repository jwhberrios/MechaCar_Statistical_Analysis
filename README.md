# MechaCar_Statistical_Analysis
Auto Production Data Analysis Using R to perform linear regression test, t-tests, and create summary statistics of production data on an autopmobile prototype.

## Linear Regression to Predict MPG
A linear regression test was performed using the following variables to predict MPG:
* Vehicle length
* Vehicle weight
* spoiler angle
* ground clearance
* AWD

The results are presented below in figure 1.

![figure 1. Linear Regression to Predict MPG](https://github.com/jwhberrios/MechaCar_Statistical_Analysis/blob/main/Resources/MLR_output.png)

figure 1. Linear regression to predict MPG result output

### Results
Based on the result output for the linear regression test, vehicle length, ground clearance, and the y-intercept were found to be statistically significant in contributing to the variance to the MPG variable with a p value < 0.05.

The slope of this linear model is not considered to be zero becuase the R squared value is 0.71. Since this R squared value indicates a strong relationship and a statistically siginficant relationship (p < 0.05) exists between some variables (vehicle length and ground clearance) used in this regression test to predict MPG, this linear model can predict MPG of MechaCar prototypes effectively.


## Summary Statistics on Suspension Coils
The mean, meadian, variance, and standard deviation was calculated using suspension coil data that was provided. The summary statistic of the data is presented in figure 2 and the summary statistic per lot is presented in figure 3.

![figure 2. Summary statistic table](https://github.com/jwhberrios/MechaCar_Statistical_Analysis/blob/main/Resources/Coil_summary_table.png)

figure 2. Summary statistic table 



![figure 3. Summary statistic table per lot](https://github.com/jwhberrios/MechaCar_Statistical_Analysis/blob/main/Resources/Summary_lot_table.png)

figure 3. Summary statistic table per lot

### Results
With the design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch, the mean and standard deviation presented in figure 2 (1498.78 PSI, SD = 0.99) and the mean PSI and standard deviation for each lot presented in figure 3 indicates the suspension coil during production significantly exceeds the 100 pounds per square inch design specification.

As such, based on this data analyses, the current manufacturing data does not meet the design specifications for all manufacturing lots in total and each lot individually. 


## T-Tests on Suspension Coils
T-tests were performed to determine if all manufacturing lots and each lot individually were statistically different from the population mean of 1,500 pounds per square inch.
The results of the simple student t-test to determine if all manufacturing lots were statistically different from the population mean of 1,500 pounds per square inch are presented in figure 4. A multiple t-test analyzing data for each lot individually are presented in figure 5.




