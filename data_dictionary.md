# Credit Card Customer Segmentation Dataset Documentation

## Overview

This dataset is designed for customer segmentation analysis in the credit card industry. It contains customer demographic information, account behavior metrics, and transaction patterns that can be used to identify distinct customer segments and tailor marketing strategies.

## Data Structure

- **Number of Records**: 20
- **Number of Features**: 13
- **File Format**: CSV
- **Last Updated**: April 2025

## Feature Descriptions

### 1. Customer Identifiers

| Feature Name | Type    | Description                | Example Values |
| ------------ | ------- | -------------------------- | -------------- |
| customer_id  | Integer | Unique customer identifier | 1001-1020      |

### 2. Demographic Information

| Feature Name    | Type    | Description                | Valid Values/Range   |
| --------------- | ------- | -------------------------- | -------------------- |
| age             | Integer | Customer's age in years    | 22-50                |
| gender          | String  | Customer's gender          | M, F                 |
| dependent_count | Integer | Number of dependents       | 0-4                  |
| education_level | String  | Highest education achieved | See categories below |
| marital_status  | String  | Marital status             | See categories below |

#### Education Level Categories

- **Uneducated**: No formal education
- **High School**: Secondary education completed
- **College**: Some college education
- **Graduate**: Bachelor's degree completed
- **Post-Graduate**: Master's level education
- **Doctorate**: PhD or equivalent degree

#### Marital Status Categories

- **Single**: Never married
- **Married**: Currently married
- **Divorced**: Previously married, now divorced
- **Unknown**: Status not disclosed/available

### 3. Financial Information

| Feature Name     | Type    | Description             | Range/Units        |
| ---------------- | ------- | ----------------------- | ------------------ |
| estimated_income | Integer | Projected annual income | 25,000-150,000 USD |

### 4. Account Behavior

| Feature Name             | Type    | Description                  | Range        |
| ------------------------ | ------- | ---------------------------- | ------------ |
| months_on_book           | Integer | Customer tenure              | 12-72 months |
| total_relationship_count | Integer | Number of bank interactions  | 1-5 contacts |
| months_inactive_12_mon   | Integer | Inactive months in last year | 1-4 months   |

### 5. Transaction Patterns

| Feature Name          | Type    | Description              | Range/Units         |
| --------------------- | ------- | ------------------------ | ------------------- |
| total_trans_amount    | Float   | Total transaction value  | 300.00-5,200.25 USD |
| total_trans_count     | Integer | Number of transactions   | 10-50 transactions  |
| avg_utilization_ratio | Float   | Credit utilization ratio | 0.36-0.57           |

## Data Quality Notes

1. **Completeness**

   - No missing values in any field
   - All records have valid entries across all features

2. **Consistency**

   - All monetary values are in USD
   - All time-based metrics are in months
   - Education levels follow a clear hierarchical structure
   - Marital status categories are mutually exclusive

3. **Value Constraints**
   - All numeric fields contain positive values
   - Utilization ratios are properly bounded (0-1)
   - Age values are realistic for credit card holders
   - Income values align with education levels

## Usage Guidelines

1. **Preprocessing Recommendations**

   - Convert categorical variables using appropriate encoding
   - Scale numeric features before clustering
   - Consider feature importance when selecting variables

2. **Analysis Considerations**
   - Account for income-education correlation
   - Consider demographic balance in segmentation
   - Factor in both monetary and behavioral patterns

## Additional Notes

- Regular transaction patterns may indicate customer loyalty
- Utilization ratio can signal financial behavior
- Relationship count suggests engagement level
- Inactive months may indicate churn risk
