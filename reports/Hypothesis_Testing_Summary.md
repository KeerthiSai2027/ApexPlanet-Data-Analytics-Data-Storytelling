# Hypothesis Testing Summary: Credit Risk Analysis

## 1. Overview

In Task 4, we move beyond exploratory data analysis to validate our observations with statistical rigor. The core goal is to determine if identified differences between risk segments are statistically significant or merely due to random chance.

## 2. Methodology

We utilized an **Independent T-Test** to compare the means of a specific variable across two independent groups (e.g., High Risk vs. Low Risk customers).

- **Test:** Independent Sample T-Test
- **Confidence Level:** 95% ($ lpha = 0.05$)
- **Tool:** `scipy.stats.ttest_ind`

## 3. Hypothesis Formulation

- **Null Hypothesis (H₀):** There is no significant difference in the mean [Variable] between High Risk and Low Risk segments.
- **Alternative Hypothesis (H₁):** There is a statistically significant difference in the mean [Variable] between the segments.

## 4. Key Metrics to Report

When presenting your findings, you must report these three values:

1. **T-Statistic:** Measures the size of the difference relative to the variation in your sample data.
2. **P-Value:** The probability of observing these results if the Null Hypothesis were true.
   - If **p < 0.05**, reject H₀ (Result is significant).
   - If **p > 0.05**, fail to reject H₀ (Result is not significant).
3. **Mean Comparison:** The actual average difference between the two groups (e.g., "High-risk customers have, on average, $X lower income than low-risk customers").

## 5. Interpreting the Results

[Image of t-test normal distribution and p-value threshold]

- **If p < 0.05:** You have successfully validated that your segmentation model (Task 3) identifies real, actionable differences in customer behavior.
- **Strategic Implication:** This result justifies focusing resources on specific high-risk segments, as the differences are confirmed to be robust.

## 6. Template for your Submission

| Variable     | Segment 1 | Segment 2 | T-Stat  | P-Value | Conclusion              |
| :----------- | :-------- | :-------- | :------ | :------ | :---------------------- |
| Income       | High Risk | Low Risk  | [Value] | [Value] | [Reject/Fail to Reject] |
| Credit Score | High Risk | Low Risk  | [Value] | [Value] | [Reject/Fail to Reject] |

---

_Task 4: Statistical Validation documentation prepared for ApexPlanet._

Hypothesis_Testing_Summary.md
Displaying Hypothesis_Testing_Summary.md.
