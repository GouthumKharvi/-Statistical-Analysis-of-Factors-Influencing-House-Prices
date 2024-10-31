# -Statistical-Analysis-of-Factors-Influencing-House-Prices
This study employs multiple regression analysis to evaluate the impact of price per square foot, number of bathrooms, and floor size on the price of high-floor, spacious 2-bedroom houses, testing the null hypothesis that these factors have no significant effect.

# Housing Price Analysis

## Overview
This project investigates the impact of various independent variables—price per square foot, number of bathrooms, and floor size—on the price of high-floor, spacious 2-bedroom houses with spectacular views. The analysis utilizes data provided in an Excel file to conduct multiple regression analysis.

## Hypotheses

- **Null Hypothesis (H0)**: There is no significant effect of the independent variables on the price.
- **Alternative Hypothesis (H1)**: There is a significant effect of the independent variables on the price.

## Confidence Level
A **95% confidence level** is selected for this analysis, meaning we can expect the true parameter value to fall within this range 95% of the time.

## Statistical Model
To test the hypotheses, **multiple regression analysis** is employed. This statistical method helps determine the relationship between the dependent variable (price) and the independent variables (price per square foot, number of bathrooms, and floor size).

## Data Summary

### Descriptive Statistics
- **Price**
  - Mean: $90,035.54
  - Median: $85,000
  - Mode: $85,000
  - Standard Deviation: $18,789.33
  - Minimum: $62,500
  - Maximum: $184,000

- **Floor Size**
  - Mean: 1,320.99 sq ft
  - Median: 1,308 sq ft
  - Mode: 1,163 sq ft
  - Standard Deviation: 226.66 sq ft
  - Minimum: 678 sq ft
  - Maximum: 2,421 sq ft

- **Price per Square Foot**
  - Mean: $68.77
  - Median: $66.38
  - Mode: $75.69
  - Standard Deviation: $11.57
  - Minimum: $45.07
  - Maximum: $111.03

### Confidence Intervals
- **95% Confidence Level**:
  - Price: ±$1,952.96
  - Floor Size: ±23.56 sq ft
  - Price per Square Foot: ±$1.20

## Regression Analysis

### Summary Output
- **Multiple R**: 0.9926
- **R Square**: 0.9852
- **Adjusted R Square**: 0.9850
- **Standard Error**: $2,297.77
- **Observations**: 358

### ANOVA Results
| Source        | df  | SS           | MS              | F          | Significance F |
|---------------|-----|--------------|-----------------|------------|-----------------|
| Regression    | 3   | 1.24166E+11 | 41,388,611,948  | 7839.14    | 0               |
| Residual      | 354 | 1,869,027,113| 5,279,737.608   |            |                 |
| Total         | 357 | 1.26035E+11 |                 |            |                 |

### Coefficients
| Variable         | Coefficient      | Standard Error | t Stat      | P-value       | 95% Confidence Interval       |
|------------------|------------------|-----------------|-------------|---------------|-------------------------------|
| Intercept        | -97,558.76       | 1,269.71        | -76.84      | 7.05E-223     | [-100,055.89, -95,061.63]    |
| Floor Size       | 69.70            | 0.65            | 107.59      | 1.75E-272     | [68.43, 70.97]                |
| No. of Bathrooms  | 496.99           | 245.69          | 2.02        | 0.0438        | [13.78, 980.20]              |
| Price per Sq Ft  | 1,368.67         | 11.10           | 123.36      | 5.83E-293     | [1,346.85, 1,390.50]         |

## Conclusion
The regression analysis reveals a strong relationship between the independent variables and the price. The P-values for all predictors are less than 0.05, allowing us to reject the null hypothesis and conclude that there are statistically significant effects of the independent variables on the price of the property.

## Future Work
Future analysis could consider additional variables such as location, property age, and amenities to further refine the model's predictive capabilities.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
