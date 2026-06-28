# KPI Framework, Business Experiment Analysis & Decision Recommendation

## Student Information

- **Name:** Ansh Raj
- **Student ID:** Bitsom_ba_2511049

---

# Business Context

A subscription-based digital product company launched a new onboarding and activation campaign to improve user conversion and early engagement.

Users were randomly divided into two groups:

- **Control Group:** Existing onboarding experience
- **Treatment Group:** New onboarding campaign

The objective of this experiment was to determine whether the new onboarding experience should be launched to all users based on data-driven analysis.

---

# Business Problem Statement

The company needs to decide whether the new onboarding campaign should replace the existing onboarding experience.

This decision impacts:

- Product Team
- Marketing Team
- Business Leadership
- Customers

The primary goal is to improve the **Paid Conversion Rate** while ensuring that user experience and business quality are not negatively affected.

Before making the recommendation, statistical evidence and guardrail metrics must be evaluated.

---

# Dataset Description

Dataset Name:

`campaign_experiment_data.xlsx`

The dataset contains user-level experiment data including:

- User ID
- Experiment Group
- Landing Page Visit
- Trial Started
- Onboarding Completed
- Paid Conversion
- Revenue
- Refund Request
- Support Ticket
- Engagement Score
- Days to Convert
- Region
- Device Type
- Traffic Source
- Plan Type

---

# Data Cleaning & Preparation

The dataset was cleaned before analysis.

The following checks were performed:

- Checked for missing values
- Verified experiment group counts
- Checked duplicate User IDs
- Validated binary columns (0/1)
- Reviewed revenue outliers
- Verified segment distribution
- Ensured consistent data types

No major data quality issues affecting the analysis were found.

---

# North Star Metric

**Paid Conversion Rate**

## Why this metric?

Paid Conversion Rate directly measures the percentage of users who become paying customers.

Improving this metric directly increases subscription revenue and business growth.

---

# Supporting KPIs

- Landing Page Visit Rate
- Trial Start Rate
- Onboarding Completion Rate
- Average Revenue Per User (ARPU)
- Average Revenue Per Converted User (ARPPU)
- Engagement Score
- Days to Convert

---

# Guardrail Metrics

The following guardrail metrics were evaluated:

- Refund Rate
- Support Ticket Rate
- Average Days to Convert
- Engagement Score

These metrics ensure that conversion improvements do not negatively impact customer experience.

---

# KPI Tree Summary

North Star Metric

→ Paid Conversion Rate

Primary Drivers

- Landing Page Visit Rate
- Trial Start Rate
- Onboarding Completion Rate

Supporting Metrics

- Engagement Score
- Revenue
- Conversion Speed

Guardrail Metrics

- Refund Rate
- Support Ticket Rate
- Engagement Score

---

# Experiment Analysis Approach

The following analyses were performed:

- Data Cleaning
- KPI Calculation
- Pivot Table Analysis
- Segment-wise Analysis
- Experiment Summary
- A/B Test
- Guardrail Metric Evaluation

---

# Hypothesis Test Summary

### Null Hypothesis (H₀)

There is no significant difference in Paid Conversion Rate between the Control and Treatment groups.

### Alternative Hypothesis (H₁)

The Treatment group has a significantly higher Paid Conversion Rate.

### Test Used

Two-Sample t-Test (Unequal Variances)

### Significance Level

0.05

### Results

- Control Mean = 3.19%
- Treatment Mean = 7.04%
- p-value = 0.001026

Since the p-value is less than 0.05, the Null Hypothesis was rejected.

The Treatment group showed a statistically significant improvement.

---

# Experiment Findings

| Metric | Control | Treatment |
|---------|---------|-----------|
| Paid Conversion Rate | 3.19% | 7.04% |
| ARPU | 51.97 | 54.25 |
| ARPPU | 1630.10 | 770.41 |
| Refund Rate | 0.00% | 0.42% |
| Support Ticket Rate | 0.2203 | 0.3732 |
| Engagement Score | 57.03 | 62.94 |
| Days to Convert | 8.86 | 6.40 |

---

# Final Recommendation

**Recommendation: Launch the New Onboarding Campaign**

Reason:

- Paid Conversion Rate increased significantly.
- User engagement improved.
- Users converted faster.
- Statistical testing confirmed the improvement.
- Guardrail metrics showed acceptable business risk.

---

# Assumptions & Limitations

- Results are based on the provided dataset.
- Long-term customer retention was not analyzed.
- Future experiments may produce different outcomes.
- Support ticket rate should continue to be monitored after launch.

---

# Repository Structure

```
part2_kpi_experiment/
│
├── data/
├── analysis/
├── outputs/
├── screenshots/
└── README.md
```

---

# Screenshots Included

The repository contains the following screenshots:

- ✅ summary_metrics.png
- ✅ hypothesis_test_output.png
- ✅ kpi_tree_preview.png

---

# Tools Used

- Microsoft Excel
- Pivot Tables
- Statistical Hypothesis Testing
- GitHub
- Markdown

---

# Conclusion

The experiment demonstrates that the Treatment onboarding campaign significantly improves Paid Conversion Rate while maintaining acceptable business performance across key guardrail metrics.

Based on statistical evidence and business analysis, the recommendation is to launch the new onboarding experience.