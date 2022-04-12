# MechaCar_Statistical_Analysis
Auto Production Data Analysis Using R and RStudio to perform linear regression test, t-tests, and create summary statistics of production data on an automobile (MechaCar) prototype.

## Muiltiple Linear Regression to Predict MPG
A multiple linear regression test was performed using the following variables to predict MPG:
* Vehicle length
* Vehicle weight
* spoiler angle
* ground clearance
* AWD

The results are presented below in figure 1.

![figure 1. Multiple Linear Regression to Predict MPG](https://github.com/jwhberrios/MechaCar_Statistical_Analysis/blob/main/Resources/MLR_output.png)

**figure 1. Multiple Linear regression to predict MPG result output**

--------------------------------------------------------------------------

### Results
Based on the result output for the linear regression test, vehicle length, ground clearance, and the y-intercept were found to be statistically significant in contributing to the variance to the MPG variable with a p value < 0.05.

The slope of this linear model is not considered to be zero becuase the R squared value is 0.71. Since this R squared value indicates a strong relationship and a statistically siginficant relationship (p < 0.05) exists between some variables (vehicle length and ground clearance) used in this regression test to predict MPG, this linear model can predict MPG of MechaCar prototypes effectively.


## Summary Statistics on Suspension Coils
The mean, meadian, variance, and standard deviation was calculated using suspension coil data that was provided. The summary statistic of the data is presented in figure 2 and the summary statistic per lot is presented in figure 3.

![figure 2. Summary statistic table](https://github.com/jwhberrios/MechaCar_Statistical_Analysis/blob/main/Resources/Coil_summary_table.png)

**figure 2. Summary statistic table** 

---------------------------------------------------------------

![figure 3. Summary statistic table per lot](https://github.com/jwhberrios/MechaCar_Statistical_Analysis/blob/main/Resources/Summary_lot_table.png)

**figure 3. Summary statistic table per lot**

### Results
With the design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch, the variance presented in figure 2 is below 100 PSI. The variance for each lot presented in figure 3 indicates the suspension coil during production does not exceed design specifications for lots 1 & 2. However, lot 3 shows a variance greater than 100 (170 PSI).

As such, based on this data analyses, the current manufacturing data meets the design specifications for all manufacturing lots in total. For each individual lots, lot 3 failed to meet the 100 PSI maximum variance in suspension coil.


## T-Tests on Suspension Coils
T-tests were performed to determine if all manufacturing lots and each lot individually were statistically different from the population mean of 1,500 pounds per square inch.
The results of the simple student t-test to determine if all manufacturing lots were statistically different from the population mean of 1,500 pounds per square inch are presented in figure 4. A multiple t-test analyzing data for each lot individually are presented in figure 5.

![figure 4. One sample t-test results for all manufacturing lots](https://github.com/jwhberrios/MechaCar_Statistical_Analysis/blob/main/Resources/One%20sample%20t-test.png)

**figure 4. T-test results for all manufacturing lots**

----------------------------------------------------------------------------

![figure 5. Multiple t-test results comparing each individual lots](https://github.com/jwhberrios/MechaCar_Statistical_Analysis/blob/main/Resources/Mulitple_t_test.png)

**figure 5. Multiple t-test results comparing each individual lots**

### Results

The results for all manufacturing lots did not result in a statistically significant different mean (p <0.05) compared to the population mean. However, the mean for lot 3 in the multiple t-test yielded significantly different mean (p < 0.05) from the population value. It's mean of 1496.14 PSI is statitistically less than the population mean of 1500 PSI.


## Study Design: MechaCar vs Competition

In this study, the statement of the problem is how does MechaCar's drivetrain (AWD vs 2WD) compare to other competitor vehicle's drivetrain on annual maintenance cost? The metrics to test will be the mean, median, and standard deviation of annual maintenance cost for MechaCar with AWD and 2WD drivetrains and its competitor's automobiles with AWD and 2WD drivetrains.
The null hypothesis would be there will no difference in maintenance cost between MechaCars with AWD and 2WD drivetrain and its competitor's vehicles with AWD and 2WD drivetrains.

The first alternative hypothesis is a significant difference will be observed in annual maintenance cost between MechaCars with AWD compared to its competitor's vehicles with AWD.
The second alternative hypothesis is a significant difference will be observed in annual maintenance cost between MechaCars with 2WD compared to its competitor's vehicles with 2WD.

The statistical test to run this analysis will be a 2x2 ANOVA test because the independent variable is a two level categorical variable (MechaCar Vs Competitor's Vehicles; AWD vs 2WD drivetrain) and the dependent variable is continuous (annual maintenance cost). The overall analysis is looking for statistical differences in means between more than 2 sample groups.

In order to run this analysis, the data to be used would be the annual maintenance cost between vehicles (MechaCar and its competitor's vehicles) that have full time  AWD options and those with 2WD options only.

