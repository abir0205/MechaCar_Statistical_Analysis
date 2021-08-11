# MechaCar_Statistical_Analysis

## Overview of Analysis

This project aims to analyze the problems production troubles that are blocking the AutosRUs manufacturing team’s progress. The analyst's job was to:

- Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population
- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

## Linear Regression to Predict MPG
- Vehicle Length and Ground Clearance are shown to have the most statistical significance in the model, resulting in p-values of 2.6e-12 and 5.21e-8, respectively.The intercept was also statistically significant, indicating that there are likely other factors, not included in our dataset, that have a strong impact on the MPG
- The slope of this model is not zero as the R-squared value is 0.7149 and the p-value is 5.35e-11, indicating that the null hypothesis is rejected and there is a statistically significant relationship between our variables and the MPG.
- This model can be used as a predictor of MPG for this dataset as there is an R-squared value is 0.7149, which indicates a strong statistical relationship, although this cannot be taken as a universal truth as there is still room for error.
- Data from the linear regression analysis in R can be found in the images folder.

## Summary Statistics on Suspension Coils

- While the overall variance is under 100 psi and meets specifications, there is a problem with one of the individual lots. As shown in the Lot Summary stats, the variance for Lot 3 is well over the acceptable threshold, at 170.28.

## T-Tests on Suspension Coils
-  The results of the T-test for the suspension coils across all manufacturing lots shows that they are not statistically different from the population mean, and the p-value is not low enough (0.0603) for us to reject the null hypothesis, indicating there is no statistical significance.
- The T-Tests from Lot 1 and Lot 2 have p-values that are not low enough to reject the null hypothesis, meaning they are not statistically significant.
- The T-test for the suspension coils for Lot 3 shows that they are slightly statistically different from the population mean, and the p-value is just low enough (0.0417) for us to reject the null hypothesis. This lot may be need to be discarded, or at least more closely evaluated.

## Study Design: MechaCar vs. Competition
As cars become more advanced, consumers will consider more variables when they are deciding which car to buy. In order to optimize sales, AutosRUs vehicles must provide something or multiple things that make it advantageous compared to other vehicles. Many consumers will consider whether MPG, size of vehicle, and horsepower are related when buying a car. We can test how all of these attributes of AutosRUs vehicles compare to vehicles of other makes.

### Metrics
- MPG
- Size of vehicle
- Horsepower
### Null Hypothesis
A combination of these variables have no statistically significant on consumers' purchase of vehicles

### Alternate Hypothesis
A combination of these variables does have a statistically significant on consumers' purchase of vehicles

### Statistical Test
- To test this hypothesis, a two-way ANOVA would need to be used because there are more variables being tested and multiple samples that will be tested.
- To test this, we would need the MPG, size of vehicle, and horsepower of sample AutosRUs vehicles as well as the MPG, size of vehicle, and horsepower of large variety of other makes.
