# Marketing Campaign Performance and Customer Behavior Analysis

## Project Overview

This project focuses on analyzing customer demographics, purchasing behavior, product preferences, and marketing campaign performance using Python.

The main objective is to identify customer spending patterns, evaluate campaign acceptance rates, understand preferred purchasing channels, and generate actionable business recommendations.

The project also uses statistical hypothesis testing to examine whether customers who accepted the latest marketing campaign spend significantly more than those who did not.

## Dataset

- **Dataset Name:** Marketing Campaign Results
- **Source:** [Maven Analytics – Data Playground](https://mavenanalytics.io/data-playground/marketing-campaign-results)
- **Dataset Size:** 2,240 customer records
- **Data Type:** Customer demographics, product purchases, and marketing campaign responses
- **License:** Public Domain (as listed by Maven Analytics)

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook
- VS Code

## Project Objectives

1. Clean and prepare the customer dataset.
2. Analyze customer demographics and purchasing behavior.
3. Identify top-performing product categories.
4. Analyze customer preferences across purchasing channels.
5. Evaluate historical and latest marketing campaign performance.
6. Compare campaign response rates across customer groups.
7. Perform statistical hypothesis testing.
8. Generate actionable business recommendations.

## Data Cleaning & Preparation

- Checked missing values and duplicate records.
- Converted customer registration dates into datetime format.
- Identified and handled suspicious income values.
- Replaced missing income values using median imputation.
- Identified unrealistic customer ages.
- Grouped uncommon marital status categories into "Other".
- Created new features:
  - `Age`
  - `Total_Spending`
  - `Total_Purchases`

## Exploratory Data Analysis

The analysis covers:

- Customer age and income distribution.
- Customer spending patterns.
- Product category performance.
- Purchase channel analysis.
- Historical campaign acceptance.
- Latest campaign response analysis.
- Age-wise and education-wise campaign response rates.

## Key Findings

- Wines generated the highest spending among all product categories.
- Meat products ranked second in total spending.
- Store purchases were the most frequently used purchasing channel.
- Campaign 4 had the highest historical acceptance rate at 7.46%.
- The latest campaign response rate was 14.91%.
- Customers aged 65+ showed the highest observed response rate (19.48%), although this group had only 77 customers.
- PhD customers had the highest observed campaign response rate (20.78%).

## Statistical Hypothesis Testing

**Research Question:**

Do customers who accept the latest marketing campaign spend significantly more than customers who do not accept it?

| Metric | Result |
|---|---:|
| Average spending of responders | 987.39 |
| Average spending of non-responders | 538.93 |
| Difference in average spending | 448.46 |
| T-statistic | 10.8503 |
| P-value | 1.50 × 10⁻²⁴ |

**Test Used:** Welch's Independent Samples t-test (One-tailed)

**Conclusion:** The null hypothesis was rejected at the 5% significance level. Customers who accepted the latest campaign had significantly higher average spending in this dataset. However, this association does not prove that campaign acceptance caused higher spending.

## Business Recommendations

1. Study the strategy and communication used in successful marketing campaigns.
2. Focus on customer preferences for high-performing product categories.
3. Continue supporting the store channel while exploring opportunities to improve online purchases.
4. Use customer spending patterns to identify potential retention and loyalty opportunities.
5. Evaluate campaigns using revenue, profit, conversion, and customer retention metrics.

## Project Structure

```text
Marketing_Campaign_Analysis/
│
├── data/
│   ├── raw/
│   │   └── marketing_campaign.csv
│   │
│   └── processed/
│
├── notebooks/
│   └── Marketing_Campaign_Analysis.ipynb
│
├── reports/
│
└── README.md
```

## Conclusion

This project demonstrates how Python-based exploratory data analysis and statistical hypothesis testing can help understand customer behavior and marketing campaign performance.

The findings provide useful insights into customer spending, product preferences, purchasing channels, and campaign responses, supporting more informed marketing decisions.

---

**Project Type:** Data Analytics | Exploratory Data Analysis | Statistical Analysis

**Created using:** Python and Jupyter Notebook