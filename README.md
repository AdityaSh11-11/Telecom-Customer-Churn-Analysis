# Telecom Customer Churn Analysis

## Project Overview

Customer churn is one of the most critical business challenges in subscription-based industries. This project focuses on analyzing customer churn data from a telecom company to identify the key factors influencing customer attrition and provide actionable business insights for improving customer retention.

Through Exploratory Data Analysis (EDA), various customer demographics, service subscriptions, billing information, and contract details were analyzed to understand patterns associated with churn.

---

## Objective

The primary objectives of this project are:

- Analyze customer behavior and churn patterns.
- Identify factors contributing to customer attrition.
- Discover customer segments with high churn risk.
- Generate actionable insights to improve customer retention strategies.
- Build a strong foundation for future predictive churn modeling.

---

## Dataset Information

### Dataset Summary

| Metric | Value |
|----------|----------|
| Total Customers | 7,043 |
| Features | 21 |
| Missing Values | 0 |
| Duplicate Records | 0 |
| Target Variable | Churn |

### Dataset Features

#### Customer Demographics
- Gender
- Senior Citizen
- Partner
- Dependents

#### Account Information
- Tenure
- Contract Type

#### Services Subscribed
- Phone Service
- Multiple Lines
- Internet Service
- Online Security
- Online Backup
- Device Protection
- Tech Support
- Streaming TV
- Streaming Movies

#### Billing Information
- Monthly Charges
- Total Charges
- Payment Method
- Paperless Billing

#### Target Variable
- Churn (Yes/No)

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Data Preprocessing

The following preprocessing steps were performed:

### 1. Data Cleaning
- Checked for missing values.
- Checked for duplicate records.
- Verified data consistency.

### 2. Total Charges Conversion
- Replaced blank values with 0.
- Converted TotalCharges from string to float.

### 3. Senior Citizen Transformation
Converted binary values:

| Original | Converted |
|----------|----------|
| 0 | No |
| 1 | Yes |

---

## Exploratory Data Analysis

### Churn Distribution

| Status | Count | Percentage |
|----------|----------|----------|
| Retained Customers | 5,174 | 73.46% |
| Churned Customers | 1,869 | 26.54% |

### Key Finding

Approximately **1 in every 4 customers leaves the company**, indicating a significant churn challenge.

---

## Analysis Performed

### 1. Gender Analysis

#### Observation
- Male and Female customers exhibit similar churn behavior.
- Gender has minimal impact on churn.

#### Insight
Gender is not a strong predictor of customer attrition.

---

### 2. Senior Citizen Analysis

#### Observation
- Senior citizens represent a smaller customer segment.
- Their churn rate is noticeably higher than non-senior customers.

#### Insight
Senior citizens constitute a higher-risk customer group.

---

### 3. Tenure Analysis

#### Observation
- Customers with low tenure show significantly higher churn.
- Long-term customers demonstrate greater loyalty.

#### Insight
Customer retention efforts should focus on the initial months of service.

---

### 4. Contract Type Analysis

| Contract Type | Churn Risk |
|--------------|------------|
| Month-to-Month | High |
| One-Year | Medium |
| Two-Year | Low |

#### Insight
Long-term contracts significantly reduce churn probability.

---

### 5. Internet Service Analysis

#### Observation
- Fiber Optic users exhibit higher churn rates.
- DSL customers tend to remain more loyal.
- Customers without internet services show lower churn.

#### Insight
Internet service experience may influence retention.

---

### 6. Payment Method Analysis

#### Observation
Customers using:
- Electronic Check → Highest churn rate

Customers using:
- Credit Card (Automatic)
- Bank Transfer (Automatic)

show lower churn rates.

#### Insight
Automatic payment methods improve customer retention.

---

### 7. Additional Service Analysis

The following services were analyzed:

- Online Security
- Online Backup
- Device Protection
- Tech Support
- Streaming TV
- Streaming Movies

#### Findings

Customers lacking:

❌ Online Security  
❌ Online Backup  
❌ Device Protection  
❌ Tech Support  

are significantly more likely to churn.

Customers subscribed to these services show stronger retention.

---

## Key Business Insights

### Major Drivers of Churn

| Factor | Impact |
|----------|----------|
| Month-to-Month Contract | 🔴 High |
| Low Tenure | 🔴 High |
| Senior Citizen Status | 🔴 High |
| Electronic Check Payments | 🔴 High |
| No Online Security | 🔴 High |
| No Tech Support | 🔴 High |
| No Device Protection | 🔴 High |

### Factors Reducing Churn

| Factor | Impact |
|----------|----------|
| Two-Year Contracts | 🟢 Positive |
| One-Year Contracts | 🟢 Positive |
| Automatic Payments | 🟢 Positive |
| Security Services | 🟢 Positive |
| Technical Support | 🟢 Positive |

---

## Project Outcomes

### Churn Rate
**26.54%**

### Customer Retention Rate
**73.46%**

### High-Risk Customer Segments

- New Customers
- Month-to-Month Contract Holders
- Senior Citizens
- Electronic Check Users
- Customers without Security & Support Services

---

## Recommendations

### 1. Encourage Long-Term Contracts
Offer discounts and loyalty incentives for annual plans.

### 2. Improve Customer Onboarding
Focus on customer engagement during the first few months.

### 3. Promote Automatic Payments
Provide incentives for auto-payment enrollment.

### 4. Bundle Value-Added Services
Include:
- Online Security
- Tech Support
- Device Protection

in retention packages.

### 5. Target High-Risk Segments
Develop personalized retention campaigns for:
- Senior Citizens
- New Customers
- Month-to-Month Subscribers

---

## Visualizations Included

- Churn Distribution
- Gender vs Churn
- Senior Citizen vs Churn
- Tenure Distribution
- Contract Type Analysis
- Payment Method Analysis
- Service Subscription Analysis
- Internet Service Analysis

---

## Future Improvements

- Build Machine Learning models for churn prediction.
- Perform feature engineering.
- Develop customer risk scoring.
- Create an interactive dashboard using Power BI or Tableau.
- Deploy a churn prediction web application.

---

## Project Structure

```
Customer-Churn-Analysis/
│
├── churn.ipynb
├── README.md
├── Report Summary/
│   ├── Customer Churn Analysis.pdf
└── Data/
    ├── Customer Churn.csv

```

---

## Conclusion

This project successfully identified the major factors influencing customer churn through comprehensive exploratory data analysis. The findings reveal that contract type, customer tenure, payment methods, and value-added services play a crucial role in customer retention. These insights can help businesses design effective retention strategies, reduce churn rates, and improve long-term customer satisfaction.

---

### If you found this project useful, feel free to star the repository and connect with me on LinkedIn!
