# A/B Testing: Website Redesign Impact Analysis

## Project Overview
This project evaluates the impact of a website redesign on key user engagement and conversion metrics. Using Python (Pandas, SciPy) for statistical analysis and Tableau for data visualization, I conducted a comprehensive A/B test analysis to determine if the new design (Treatment) outperforms the current one (Control).

## Key Objectives
* Evaluate the statistical significance of changes in Conversion Rate (CR).
* Analyze user engagement through Mean Session Duration and Mean Pages per Session.
* Perform segmentation analysis by age groups to identify specific behavioral patterns.
* Validate the reliability of results using confidence intervals and hypothesis testing.

## Tech Stack
* <b>Data Processing</b>: Python (Pandas, NumPy).
* <b>Statistical Analysis</b>: SciPy, Statsmodels
* <b>Visualization</b>: Tableau Public
* <b>Environment</b>: Google Colab

## Methodology
1. <b>Data Cleaning:</b> Checked for outliers and validated data integrity.
2. <b>Hypothesis Formulation:</b>  Defined Null (H0) and Alternative (H1) hypotheses for each metric (One-tailed tests).
3. <b>Statistical Testing:</b>
    * <b>Z-test</b> for Conversion Rate (proportions).
    * <b>Welch’s T-test</b> for Session Duration and Visited Pages (due to unequal variances and approximately normal distributions   guaranteed by the Central Limit Theorem).

![bandicam 2026-03-18 08-04-24-973](https://github.com/user-attachments/assets/cd7981f3-367a-4ab6-9548-ef5d94c711a9)
     
  ![bandicam 2026-03-18 08-11-37-265](https://github.com/user-attachments/assets/f506626e-e199-4a41-a7bb-a142d24ecd62)

4. <b>Segmentation:</b> Drilled down into age groups (<25, 25-34, 35-44, 45+) to assess consistency across demographics.

## Results & Insights
Based on the analysis of 10,000 sessions (approx. 5,000 per variant):
* <b>Conversion Rate:</b>  Increased from 10.65% to 14.34%. The z-statistic (5.57) exceeds the critical value (1.96), confirming statistical significance (p < 0.05).
* <b>User Engagement:</b> 
   * Average Session Duration grew from 5.03 to 7.02 minutes.
   * Average Pages Visited increased from 2.98 to 5.01.
* <b>Segment Performance:</b> The positive trend is consistent across all age groups. While the 25-34 segment showed a smaller absolute CR lift (2%) and p-value > 0.05(the difference is insignificant), the overall engagement metrics remained strong.

## Dashboard
The interactive visualization was created in Tableau and includes:
* Summary cards with test statistics (z-score, t-score).
* Bar charts with 95% Confidence Intervals (CI).
* Age-group breakdown for granular analysis.

👉 [Link to Tableau Public Dashboard](https://public.tableau.com/views/ABtest_17711589603130/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
<img width="1366" height="768" alt="Знімок екрана (117)" src="https://github.com/user-attachments/assets/5df2c757-90be-4dae-81d5-a4f1ce41163b" />

## Conclusion
The A/B test results provide strong evidence that the new design significantly improves both conversion and user engagement. The findings are statistically significant at the 95% confidence level, justifying a full-scale rollout of the redesign.

