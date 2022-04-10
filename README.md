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

figure 1. Linear regLression to predict MPG result output

### Results
Based on the result output for the linear regression test, vehicle length, ground clearance, and the y-intercept were found to be statistically significant in contributing to the variance to the MPG variable with a p value < 0.05.

The slope of this linear model is not considered to be zero becuase the R squared value is 0.71. Since this R squared value indicates a strong relationship and a statistically siginficant relationship (p < 0.05) exists between some variables (vehicle length and ground clearance) used in this regression test to predict MPG, this linear model can predict MPG of MechaCar prototypes effectively.


## Summary Statistics on Suspension Coils
The mean, meadian, variance, and standard deviation was calculated using suspension coil data that was provided. The summary statistic of the data is presented in figure 1 and the summary statistic per lot is presented in figure 2.

![figure 1. Summary statistic table](


