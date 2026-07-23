# A/B Testing Analysis: Impact of Advertisement Exposure on Conversion

## Project Overview

This project evaluates whether exposure to a new advertisement increases the probability that users respond positively ("yes") compared with a control group.

The analysis focuses on estimating the causal impact of the advertisement while checking whether differences in user characteristics could bias the results.

## Methodology

- Compared conversion rates between exposed and control groups.
- Estimated the treatment effect using:
  - Difference in conversion rates (absolute and relative lift).
  - Two-proportion z-test to assess statistical significance.
  - Logistic regression to estimate the effect size and adjust for potential confounders.
- Investigated possible confounding variables, including:
  - Date
  - Platform operating system
  - Browser type
- Performed sensitivity analysis by comparing:
  - Naive model: `yes ~ experiment`
  - Adjusted models including relevant covariates.

## Key Findings

- Users exposed to the advertisement had a higher conversion rate than users in the control group.
- The advertisement increased conversion by approximately **1.2 percentage points** (from ~6.5% to ~7.7%), corresponding to an **~18.6% relative improvement**.
- The difference was statistically significant using a one-sided two-proportion z-test.
- Adjusting for potential confounding variables produced similar treatment effect estimates, suggesting that the observed improvement was robust.

## Tools Used

- Python
- Pandas
- NumPy
- Statsmodels
- Scipy
- Matplotlib

## Conclusion

The analysis provides evidence that the new advertisement positively impacts user conversion. The estimated uplift is consistent across different modelling approaches, supporting the decision to consider wider deployment of the advertisement.
