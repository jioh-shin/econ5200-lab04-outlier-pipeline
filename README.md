# Outlier Detection on California Housing

## Objective

I compared different outlier detection methods on the California Housing dataset to see how each method identifies unusual observations.

## Methodology

- I diagnosed and fixed three bugs in an outlier-detection pipeline.
- I used an `OutlierDetector` class to apply modified Z-score, Tukey fences, and Isolation Forest.
- I applied modified Z-score and Tukey fences to `MedInc` and Isolation Forest to all 9 columns.
- I compared the observations flagged by the three methods and examined where their results agreed.
- I wrote a method-selection memo recommending a combination of Tukey fences and Isolation Forest.
- I built an interactive outlier method explorer to compare the methods.

## Key Findings

The modified Z-score method flagged 400 observations on `MedInc`, while Tukey fences flagged 681 observations on `MedInc`. Isolation Forest, applied to all 9 columns, flagged 1,032 observations. All three methods agreed on 322 observations. These results showed me that different outlier detection methods can identify different sets of observations, so the choice of method matters.
