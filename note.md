# Customer Churn Profile Analysis

## Project Overview

This project performs a comprehensive customer churn profiling analysis using the Telco Customer Churn dataset. The primary objective is to identify which customer segments are most likely to churn by analyzing behavioral and subscription-related patterns.

The analysis focuses entirely on business analytics and customer segmentation without using machine learning or predictive modeling techniques.

The dataset contains 7,043 customer records and 21 columns related to customer demographics, account information, services, billing behavior, and churn status.

---

# Methodology

- Loaded and explored the Telco Customer Churn dataset using pandas
- Checked dataset dimensions, column types, and missing values
- Converted `TotalCharges` into numeric format
- Removed 11 rows containing missing values
- Converted the `Churn` column into binary format:
  - Yes = 1
  - No = 0
- Calculated the overall churn rate
- Performed churn segmentation analysis across:
  - Contract types
  - Payment methods
  - Internet service categories
  - Senior citizen groups
  - Tenure groups
- Created tenure bins for customer lifecycle analysis
- Compared monthly charges between churned and retained customers
- Conducted grouped churn analysis using:
  - Contract Type
  - Internet Service
- Analyzed average tenure by contract type and churn status
- Identified high-risk customer profiles using multiple customer attributes
- Built professional visualizations using matplotlib and seaborn

---

# Key Churn Findings

- Overall churn rate is approximately **26.5%**
- Customers with **month-to-month contracts** show the highest churn rate at nearly **42.7%**
- Customers with **two-year contracts** have very low churn rates at approximately **2.8%**
- Customers within the **0–12 month tenure group** are the highest-risk segment with around **47.4% churn**
- **Fiber Optic** customers churn nearly twice as much as DSL users
- Customers using **Electronic Check** payment methods have the highest churn rate at approximately **45.3%**
- Customers with **MonthlyCharges above $65** display higher churn tendencies
- **Senior citizens** churn significantly more than non-senior customers

---

# Segment Observations

## Contract Type Analysis

Contract duration is one of the strongest indicators of customer retention. Long-term contracts are associated with significantly lower churn rates, while month-to-month subscriptions are highly unstable.

## Tenure Analysis

Customer retention improves considerably as tenure increases. Newly acquired customers are substantially more likely to churn compared to long-tenure customers.

## Internet Service Analysis

Fiber Optic customers demonstrate elevated churn rates despite being premium subscribers. This may indicate higher service expectations or pricing sensitivity.

## Payment Method Analysis

Electronic Check users show the weakest retention behavior among all payment methods, suggesting lower billing engagement and weaker customer commitment.

## Senior Citizen Analysis

Senior customers exhibit noticeably higher churn behavior, highlighting the importance of tailored customer support and retention strategies for this segment.

---

# High-Risk Customer Profiles

The highest-risk customer profiles are primarily characterized by combinations of:

- Month-to-month contracts
- Fiber Optic internet service
- Electronic Check payment method
- Short customer tenure
- Senior citizen status

These customer groups consistently demonstrate the highest churn concentration and should be prioritized for retention initiatives.

---

# Business Interpretation

The analysis reveals that customer commitment level plays a critical role in retention behavior. Customers with shorter contracts and lower tenure periods are significantly more vulnerable to churn.

Higher monthly billing amounts combined with premium internet services also contribute to increased cancellation risk. Additionally, customers using less automated payment methods appear more likely to disengage from the service.

The findings suggest that improving the early-stage customer experience and encouraging long-term engagement could significantly reduce churn levels.

---

# Retention Recommendations

1. Launch targeted onboarding and retention campaigns for customers within their first 12 months.

2. Encourage customers to transition from month-to-month plans to long-term contracts using discounts or loyalty incentives.

3. Develop dedicated support programs for senior citizens to improve customer satisfaction and engagement.

4. Offer pricing bundles or loyalty rewards for Fiber Optic customers with high monthly charges.

5. Promote automatic payment methods and provide incentives for customers to move away from Electronic Check payments.
