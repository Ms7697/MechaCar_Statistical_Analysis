# MechaCar_Statistical_Analysis

## Findings of Statistical Analysis:


## MPG REGRESSION: Interpretation of the multiple linear regression results.
1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
~ Using a multiple linear regression model, I could determine that vehicle length and ground clearance have a statistical significance on miles per gallon (mpg). Both vehicle length and ground clearance had p-values below the significance level of 0.05%. Vehicle length and ground clearance had p-values equal to 2.60e-12 and 5.21e-08, respectively.

2. Is the slope of the linear model considered to be zero? Why or why not?
~ Given that the multiple r-square value is 0.7149 and the p-value is below the significance level of 0.05%, there is sufficient evidence to reject the null hypothesis, which means that the slope of the linear model is not zero.

3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
~ The linear model is a good indicator of effectiveness because the multiple r-square value is 0.7149 and the p-value is 5.35e-11, which is below the significance level of 0.05%. The r-square value tells me that about 71% of predictions will be correct using this linear model.



## SUSPENSION COIL SUMMARY: Interpretation and findings for the suspension coil summary statistics.
* The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per inch (PSI). 
1. Does the current manufacturing data meet this design specification? Why or why not?
~ Collectively, the manufacturing lots had a PSI variance of 62.3, which meets the design specification. However, when grouped by manufacturing lots, lots 1 and 2 met the design specification well below the PSI limit. Lot 1 had a PSI variance of 0.980 and lot 2 had a PSI variance of 7.47. Lot 3 did not meet the design specification; it exceeded the PSI limit. Summary statistics show that Lot 3 had a PSI variance of 170.



## SUSPENSION COIL T-TEST: Interpretation and findings for the t-test results.
* Determine if the suspension coil???s pound-per-inch results are statistically different from the mean population results of 1,500 pounds per inch.
~ Collectively, the p-value of the suspension coil???s PSI is 0.06028, which is above the significance level of 0.05% and therefore demonstrates that it is not statistically different (aka it is statistically similar to) from the mean population PSI results. However, when grouped by manufacturing lots, lot 1 had a p-value of 1 and lot 2 had a p-value of 0.6072, which are above the significance level as well, and thereby demonstrate that they are not statistically different from the mean population PSI results. Lot 3 had a p-value of 0.04168, which is below the significance level. Among the three manufacturing lots, the suspension coil's PSI of lot 3 is the only one that is statistically different from the mean population PSI results.



## DESIGN MY OWN STUDY:
Horsepower is a metric that can be used to compare the MechaCar prototype vehicle to other comparable vehicles on the market. Although the MechaCar dataset did not include this metric, the mtcars dataset did. I used a single linear regression model to determine whether there is a correlation between horsepower (hp) and miles per gallon (mpg). It tested the following hypotheses:
  * H0: There is a correlation between hp and mpg.
  * Ha: There is no collreation between hp and mpg.
The model resulted in a multiple r-square value of 0.6024. Given the multiple r-square value, I can see that there is a moderate/strong correlation between hp and mpg.

I used a one-sample t-test as my second statistical test. I tested on a sample size of 16 to see if there is statistical similarities between the horsepower sample mean and horsepower population mean. I did this to see if hp would be worthy data collection point for further analysis. It tested the following hypotheses:
  * H0 : There is no statistical difference between the observed sample mean and its presumed population mean.
  * Ha : There is a statistical difference between the observed sample mean and its presumed population mean.
The t-test resulted in a p-value of 0.4084, which is above the significance level of 0.05%. Therefore, I do not have sufficient evidence to reject the null hypothesis, and thereby state that the two means are statistically similar.

Based on my single linear regression model and one-sample t-test, there is evidence to suggest that horsepower would be a worthy data collection point to include in the MechaCar dataset for further studies.
