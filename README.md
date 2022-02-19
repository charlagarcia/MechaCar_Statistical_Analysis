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
