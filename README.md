# MechaCar_Statistical_Analysis

## Overview
1. Load, clean up, and reshape datasets using tidyverse in R.
2. Visualize datasets with basic plots such as line, bar, and scatter plots using ggplot2.
3. Generate and interpret more complex plots such as boxplots and heatmaps using ggplot2.
4. Plot and identify distribution characteristics of a given dataset.
5. Formulate null and alternative hypothesis tests for a given data problem.
6. Implement and evaluate simple linear regression and multiple linear regression models for a given dataset.
7. Implement and evaluate the one-sample t-Tests, two-sample t-Tests, and analysis of variance (ANOVA) models for a given dataset.
8. Implement and evaluate a chi-squared test for a given dataset.
9. Identify key characteristics of A/B and A/A testing.
10. Determine the most appropriate statistical test for a given hypothesis and dataset.

## Linear Regression to Predict MPG
The MechaCar_mpg.csv dataset contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. This linear model that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file. 

We used these variables to get the following coeffecients: vehicle length, vehicle weight, spoiler angle, ground clearance, and AWD. 
![pic1](https://github.com/charlagarcia/MechaCar_Statistical_Analysis/blob/main/resources/Screenshot%20(79).png)

All coefficients are statistically significant, except AWD.  All slopes are non-zero. he p-value shows 5.35e-11, and R-squared is 0.7149. This linear model does effectively predict MPG of MechaCar prototypes, but we can't rule out that there might be other variables that contribute to MPG that aren't included in the dataset.
![pic2](https://github.com/charlagarcia/MechaCar_Statistical_Analysis/blob/main/resources/Screenshot%20(80).png)

## Summary Statistics on Suspension Coils
The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. We created a summary statistics table to show:
  - The suspension coil’s PSI continuous variable across all manufacturing lots
  - The following PSI metrics for each lot: mean, median, variance, and standard deviation.

Summary for statistics of all the manufacturing lots:
![total_sum](https://github.com/charlagarcia/MechaCar_Statistical_Analysis/blob/main/resources/total%20summary.png)

Summary by manufactuing lot:
![lot_sum](https://github.com/charlagarcia/MechaCar_Statistical_Analysis/blob/main/resources/lot%20summary.png)

The design specifications for the MecaCar suspension coils dictate that the variance must not exceed 100psi.  The variance for the total manufacturing lot is 62, which is well within the parameters.  However, Lot 3 in particular is very high, at 170 and does not meet the specifications.


## T-Tests on Suspension Coils
Perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

T-test for all lots:
![all](https://github.com/charlagarcia/MechaCar_Statistical_Analysis/blob/main/resources/ttest%20all.png)

T-test for Lot 1:
![lot1](https://github.com/charlagarcia/MechaCar_Statistical_Analysis/blob/main/resources/ttest%20lot%201.png)

T-test for Lot 2:
![lot2](https://github.com/charlagarcia/MechaCar_Statistical_Analysis/blob/main/resources/ttest%20lot%202.png)

T-test for Lot 3:
![lot3](https://github.com/charlagarcia/MechaCar_Statistical_Analysis/blob/main/resources/ttest%20lot%203.png)

Manufacturing for manufacturing lots overall, Lot 1, and Lot 2 are not statistially different from the population mean of 1500psi.

## Study Design: MechaCar vs. Competition
Design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers.

- What metric or metrics are you going to test?
    The next metric I would test is the safety rating, as that is most often one of the biggest concerns of car-buyers.
- What is the null hypothesis or alternative hypothesis?
    The null hypothesis is that the mean of the safety rating is zero.  The alternative hypothesis is that the mean of the safety rating is NOT zero.
- What statistical test would you use to test the hypothesis? And why?
    I would use a multiple linear regression statistical summary.  This would show how the variables impact safety ratings.
- What data is needed to run the statistical test?
    A random sample of safety ratings for MechaCar and competitors would need to be collected.
