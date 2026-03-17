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
4. <b>Segmentation:</b> Drilled down into age groups (<25, 25-34, 35-44, 45+) to assess consistency across demographics.

## Results & Insights
