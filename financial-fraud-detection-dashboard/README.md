# Financial Fraud Detection Dashboard

## Overview
This Power BI dashboard analyzes financial transaction data to identify fraud patterns, understand transaction behavior, and monitor suspicious financial activity.

The dashboard provides a clear view of fraud distribution, transaction risk factors, and high-value suspicious transactions using interactive visualizations.

---

# Dashboard Pages

## 1. Financial Fraud Transaction Overview

This page provides a high-level summary of transaction activity and fraud distribution.

### Key Metrics
- **Total Transactions:** ~1,048,575  
- **Fraud Transactions:** ~1,142  
- **Fraud Rate:** **0.11%**  
- **Total Transaction Amount:** **166.37 Billion**

### Visualizations
- Fraud Transactions by Transaction Type
- Transaction Volume Distribution by Type
- Fraud vs Normal Transaction Share

### Key Insights
- Fraud transactions represent only **0.11% of total transactions**, showing that fraud detection requires identifying rare anomalies.
- Most fraudulent activity occurs in **TRANSFER** and **CASH_OUT** transactions.
- **PAYMENT transactions dominate total volume**, but rarely contain fraud.

---

## 2. Fraud Risk Analysis

This page focuses on identifying risk patterns and transaction behaviors associated with fraud.

### Key Metrics
- **Fraud Rate:** 0.11%
- **Average Fraud Transaction Amount:** **1.19 Million**
- **Average Normal Transaction Amount:** **157.54 Thousand**

### Visualizations
- Fraud Distribution by Transaction Size
- Fraud Rate by Transaction Type
- Fraud vs Normal Transaction Amount Comparison

### Key Insights
- **TRANSFER transactions have the highest fraud rate (~0.65%)**, making them the most risky transaction type.
- **Large transactions account for the majority of fraud cases** (over 800 fraud transactions).
- Fraud transactions are **approximately 7.5× larger on average than normal transactions**, indicating abnormal financial behavior.

---

## 3. Financial Fraud Monitoring

This dashboard focuses on monitoring fraud activity trends and identifying suspicious high-value transactions.

### Visualizations
- Fraud Transaction Trend Over Time
- Total Transaction Amount by Transaction Type
- High Value Suspicious Transactions Table

### Key Insights
- Fraud activity shows **spikes during certain transaction steps**, indicating potential fraud bursts.
- **CASH_OUT transactions account for the highest financial outflow (~69B)**.
- **TRANSFER transactions follow closely (~55B)** and are also associated with the highest fraud rate.
- Monitoring **high-value transactions (>1M)** helps identify suspicious financial activity early.

---

# Dashboard Features

- Interactive dashboard navigation
- Transaction filtering by **transaction type** and **transaction size**
- Fraud activity monitoring
- High-value suspicious transaction detection
- Financial transaction flow analysis

---

# Tools Used

- **Power BI** – Dashboard development and visualization  
- **DAX** – KPI calculations and measures  

---

# Key Takeaways

- Fraud detection requires identifying **rare anomalies within large transaction volumes**.
- **High-value transfers are the most common pattern associated with fraud**.
- Monitoring transaction types and financial flows can significantly improve fraud detection strategies.

---

# Dashboard 
**[Download the Power BI Dashboard](https://drive.google.com/file/d/1NlEX0j0IZf4NV5f3fuwb02-_noVBf29I/view?usp=sharing)**

File format: `.pbix`
