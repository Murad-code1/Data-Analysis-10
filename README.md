# Customer Churn Profile Analysis

## 📌 Project Overview

This project performs a comprehensive customer churn profiling analysis using the Telco Customer Churn dataset to understand which customer segments are most likely to leave the service.

The dataset contains 7,043 customer records across 21 features, including customer demographics, subscription details, billing information, internet services, and churn status.

The main objective is to identify:

- High-risk customer segments
- Contract-based churn behavior
- Payment method impact on churn
- Internet service churn patterns
- Tenure-related churn trends
- Customer retention risk factors

This project focuses entirely on analytical churn profiling without using machine learning or predictive modeling techniques.

---

## 🧹 Data Cleaning

The following preprocessing steps were applied:

- Converted `TotalCharges` column into numeric format
- Removed 11 rows containing missing values
- Verified dataset structure and data types
- Converted the `Churn` column:
  - Yes → 1
  - No → 0
- Created tenure group categories for lifecycle analysis

---

## 📊 Exploratory Churn Analysis

The analysis includes:

- Overall churn rate calculation
- Churn rate by contract type
- Churn rate by payment method
- Churn rate by internet service
- Senior citizen churn analysis
- Tenure group churn analysis
- Monthly charge comparison between churned and retained customers
- Contract and internet service grouped analysis
- Average tenure analysis by churn status
- High-risk customer profile identification

---

## 📉 Overall Churn Insights

### Key Findings

- Overall churn rate is approximately **26.5%**
- Month-to-month contract customers have the highest churn rate at nearly **42.7%**
- Two-year contract customers show very low churn rates at approximately **2.8%**
- Customers within the **0–12 month tenure group** are the highest-risk segment with around **47.4% churn**
- Fiber Optic customers churn nearly twice as much as DSL users
- Electronic Check users have the highest churn rate at approximately **45.3%**
- Customers with MonthlyCharges above **$65** show increased churn tendency
- Senior citizens churn significantly more than non-senior customers

These findings highlight strong relationships between customer commitment level, service type, billing behavior, and churn risk.

---

## 📅 Tenure Group Analysis

Customers were segmented into tenure groups:

- 0–12 Months
- 13–24 Months
- 25–48 Months
- 49–72 Months

### Key Observations

- Newly acquired customers demonstrate the highest churn behavior
- Churn decreases consistently as customer tenure increases
- Long-term customers exhibit significantly stronger loyalty and retention stability

This emphasizes the importance of improving early-stage customer experience and onboarding strategies.

---

## 🌐 Internet Service Analysis

A detailed churn comparison was performed across internet service categories.

### Key Findings

- Fiber Optic customers exhibit substantially higher churn rates
- DSL customers demonstrate stronger retention behavior
- Customers without internet services have the lowest churn exposure

The results suggest that premium service customers may have higher expectations regarding service quality and pricing value.

---

## 💳 Payment Method Analysis

Payment behavior shows strong correlation with churn risk.

### Key Findings

- Electronic Check customers experience the highest churn rates
- Automatic payment methods demonstrate stronger customer retention
- Customers using bank transfers and credit card auto-pay are more stable

This indicates that billing convenience and automated payment engagement contribute positively to retention.

---

## 👥 Customer Segment Insights

Several customer characteristics are associated with elevated churn behavior:

- Short-term contracts
- Short customer tenure
- High monthly charges
- Fiber Optic subscriptions
- Electronic Check payments
- Senior citizen status

Combining these characteristics reveals clear high-risk customer profiles that require targeted retention strategies.

---

## 🚨 High-Risk Customer Profiles

The highest-risk customer profiles primarily include combinations of:

- Month-to-month contracts
- Fiber Optic internet service
- Electronic Check payment methods
- Senior citizen customers
- 0–12 month tenure group

These customer groups consistently demonstrate the highest churn concentration and should be prioritized for proactive retention campaigns.

---

## 📊 Visualizations

The project includes:

- Bar chart for churn rate by contract type
- Tenure group churn rate visualization
- MonthlyCharges boxplot for churn comparison
- Payment method churn bar chart
- Grouped bar chart for contract type and internet service analysis

All visualizations were created using matplotlib and seaborn with professional analytical formatting.

---

## 🛠️ Technologies Used

- Python
- pandas
- matplotlib
- seaborn

---

## 🚀 Conclusion

This analysis provides valuable business insights into customer retention behavior and churn risk segmentation.

Key opportunities include:

- Reducing churn among new customers
- Encouraging long-term contract adoption
- Improving retention strategies for Fiber Optic users
- Promoting automatic payment enrollment
- Developing targeted support programs for senior citizens
- Enhancing customer onboarding experiences during the first year

The findings can help businesses design more effective retention strategies and improve long-term customer loyalty.
