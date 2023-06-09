# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

![Deliverable1]( Images/Deliverable1.png)

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

The variables that contributed a non-random amount of variance to the mpg values in the dataset were vehicle length and ground clearance. The statistical significance of these variables was determined by comparing their p-values to a predetermined alpha level of .05 with a 95% confidence level. The coefficients for vehicle weight, spoiler angle, and AWD were not statistically significant, indicating they had a random amount of variance.

- Is the slope of the linear model considered to be zero? Why or why not?

The multiple linear regression formula for mpg = -.01 + 6.267(vehicle length)+.001(vehicle weight)+.069(spoiler angle)+3.546(ground clearance)-3.411(AWD), which results in a slope.

- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

The dataset displays a strong correlation with an R-squared value of .7149, indicating its effectiveness. Nevertheless, it's important to note that R-squared alone does not determine the dataset's effectiveness, as there might be other factors not accounted for in the dataset that could be causing variations in the mpg.

## Summary Statistics on Suspension Coils

![total_summary](Images/total_summary.png)
![lot_summary](Images/lot_summary.png)

- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

The overall manufacturing lot's variance of 62 < 100 falls within the expected design specifications of remaining below 100 PSI. However, upon examining the data categorized by Lot number, Lot 3 stands out as a major contributor to the high variance, recording a variance of 170 > 100, which does not meet the design specifications. In contrast, Lot 1 and Lot 2 exhibit significantly lower variance, 1 and 7, respectively.

## T-Tests on Suspension Coils
![lots_t_test](Images/lots_t_test.png)

For the total manufacturing lots, the p-value was calculated to be .6028, while the alpha level was set to .05. Given that .60 > .05, the total manufacturing lots can be regarded as not statistically significant from the normal distribution, and normality can be assumed. The mean falls within the 95% confidence interval.

![lot1_t_test](Images/lot1_t_test.png)
With respect to Lot 1, the p-value was found to be 1 while the alpha level was set at .05. Since 1 > .05, it can be inferred that Lot 1 is not statistically significant from the normal distribution, thus normality can be assumed. The mean falls within the 95% confidence interval.

![lot2_t_test](Images/lot2_t_test.png)
Regarding Lot 2, the p-value was determined to be .6072, and the alpha level was set to .05. Since .60 > .05, it can be concluded that Lot 2 is not statistically significant from the normal distribution, and normality can be assumed. The mean falls within the 95% confidence interval.

![lot3_t_test](Images/lot3_t_test.png)
Lot 3's p-value was calculated to be .04168, with an alpha level of .05. Since .04 < .05, it can be concluded that Lot 3 is statistically significant from the normal distribution, and normality cannot be assumed. Despite this, the mean value falls within the 95% confidence interval. The mean falls within the 95% confidence interval.


## Study Design: MechaCar vs Competition
- What metric or metrics are you planning to examine?
The safety rating, horsepower, and highway fuel efficiency are the next metrics to evaluate, as they address some consumer safety concerns.

- What is the null and alternative hypothesis?
The null hypothesis is that the safety rating's mean is equal to zero, while the alternative hypothesis is that the safety rating's mean is not zero.

- Which statistical test would you use to evaluate the hypothesis, and why?
A multiple linear regression analysis would be utilized to assess how the variables impact the safety ratings for both MechaCar and its competitors.

- What data is necessary to conduct the statistical test?
To conduct the statistical test, a random sample of n > 30 for MechaCar and its competitors would be needed, which includes the safety ratings, highway fuel efficiency, and horsepower data, along with running the data through RStudio.
