# Telco Customer Churn Analysis — 500 Customers

## Project Objective
This project analyzes a 500-customer telecommunications dataset to identify churn patterns, data-quality issues, outliers, and business opportunities for reducing customer attrition.

## Dataset
- Customers analyzed: 500
- Original raw file contains 505 rows because duplicate records were intentionally included for data-cleaning practice.
- Duplicate rows detected: 5
- Missing values were intentionally introduced into selected columns.
- Final cleaned dataset: 500 unique customers.

## Data Cleaning
The following steps were performed:
1. Checked column data types.
2. Counted missing values.
3. Filled categorical missing values using the mode.
4. Filled numerical missing values using the median.
5. Detected and removed duplicate records.
6. Verified the cleaned dataset.
7. Performed IQR-based outlier analysis on TenureMonths, MonthlyCharges, and TotalCharges.

## IQR Outlier Analysis
See `iqr_outlier_analysis.csv` for exact Q1, Q3, IQR, bounds, and outlier counts.

## Key Findings

### 1. Overall churn
- Churned customers: 101
- Overall churn rate: 20.20%
- Average monthly charge: 56.83
- Average tenure: 36.46 months

### 2. Contract type
The highest churn rate is for **Month-to-month** contracts at **30.39%**.
This suggests that customers without long-term commitments are more likely to leave.

### 3. Internet service
The highest churn rate is for **Fiber optic** customers at **26.14%**.
This group should receive additional service-quality and retention attention.

### 4. Payment method
The highest churn rate is for **Electronic check** at **23.67%**.
Payment experience and customer engagement should be investigated for this segment.

### 5. Churned vs retained customers
- Average monthly charge of churned customers: 60.33
- Average monthly charge of retained customers: 55.94
- Average tenure of churned customers: 28.62 months
- Average tenure of retained customers: 38.44 months

## Business Recommendations
1. Offer incentives to month-to-month customers to move to one-year or two-year contracts.
2. Create an early-retention program for customers with short tenure.
3. Investigate service-quality complaints among high-churn internet-service customers.
4. Promote technical support and security add-ons where appropriate.
5. Review payment-method experience and encourage reliable automatic payment options.
6. Use monthly-charge and tenure-based customer segments for targeted retention campaigns.
7. Monitor churn KPIs regularly rather than relying only on overall churn rate.

## Visualizations
The project contains 8 visualizations covering:
- Overall churn
- Contract vs churn
- Monthly charges
- Tenure
- Internet service vs churn
- Payment method vs churn
- Monthly charges by churn
- Tenure by churn

## Conclusion
The analysis shows that churn is not evenly distributed across customers. Contract type, internet service, payment behavior, tenure, and monthly charges provide useful signals for identifying higher-risk customers. Data cleaning and IQR analysis improve the reliability of the analysis, while targeted retention strategies can help reduce customer loss.
