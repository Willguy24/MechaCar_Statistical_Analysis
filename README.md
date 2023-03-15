# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

The variables that contributed a non-random amount of variance to the mpg values in the dataset were vehicle length and ground clearance. The statistical significance of these variables was determined by comparing their p-values to a predetermined alpha level of .05 with a 95% confidence level. The coefficients for vehicle weight, spoiler angle, and AWD were not statistically significant, indicating they had a random amount of variance.

-Is the slope of the linear model considered to be zero? Why or why not?

The multiple linear regression formula for mpg = -.01 + 6.267(vehicle length)+.001(vehicle weight)+.069(spoiler angle)+3.546(ground clearance)-3.411(AWD), which results in a slope.

-Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

The dataset displays a strong correlation with an R-squared value of .7149, indicating its effectiveness. Nevertheless, it's important to note that R-squared alone does not determine the dataset's effectiveness, as there might be other factors not accounted for in the dataset that could be causing variations in the mpg.

