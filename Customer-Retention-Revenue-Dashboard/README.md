# 📊 CUSTOMER RETENTION & REVENUE ANALYTICS DASHBOARD

## 📝 Project Summary
This project delivers an end-to-end Power BI solution to monitor **Customer Lifetime Value (CLV)** and **Retention Health**. By analyzing 905 orders totaling **$324.24K**, I identified specific segments where loyalty is high but revenue is under-tapped. The dashboard is divided into two strategic views: Executive Performance and Customer Retention.

---

## 🖥️ EXECUTIVE PERFORMANCE OVERVIEW
This page provides a high-level pulse check on sales and customer acquisition.

### **Core KPIs**
* **Total_Customers:** 580
* **Total_Orders:** 905
* **Total_Revenue:** $324.24K
* **Average_Order_Value:** $358.27

### **Strategic Insights**
* **Total_Revenue by age_group:** The **26-35** and **36-45** groups are the primary revenue drivers, contributing nearly $137K combined.
* **Customer Mix (New vs Returning):** 58.79% of the base are new customers. Converting these into "Returning" status is the biggest growth lever for the next quarter.
* **Total_Orders by channel:** E-commerce ($171.6K) currently leads over App Mobile ($152.5K), indicating a **$19K value gap** that suggests potential UX friction in the mobile app.

---

## 📈 CUSTOMER RETENTION & VALUE ANALYSIS
This page focuses on the quality of our customer base and long-term profitability.

### **Retention & Value KPIs**
* **Repeat_Purchase_Rate_%:** 41.21%
* **Retention_Rate_%:** 27.93%
* **Orders_per_Customer:** 1.56
* **Customer_Lifetime_Value:** $559.03

### **Deep-Dive Insights**
* **Revenue by Purchase Frequency:** The **2-3 Orders** bucket is the powerhouse of the business ($176K). There is **$120K** locked in the "1 Order" segment that can be unlocked via targeted loyalty campaigns.
* **Market Value & Retention Analysis:** While Germany and France provide the highest volume, **Portugal** shows the highest retention (darkest blue gradient). Portugal represents the most stable and efficient ROI for the business.
* **Daily Retention Rate Trends:** Spotted a major retention peak of **86.67%** in early June, providing a benchmark for successful engagement periods.

---

## 🛠️ Technical Implementation
* **Data Modeling:** Followed a **Star Schema** approach to optimize filtering speed and calculation accuracy across multiple dimensions (Date, Geography, Channel).
* **Advanced Visual Logic:** * **Conditional Formatting:** Applied to the Country chart so that bar height represents **Revenue** while color represents **Retention Rate**.
    * **Slicer Optimization:** Implemented a filter on the **Year_Month** slicer to ensure only months with active sales data are visible, improving user experience.
* **DAX Development:** Created custom measures for **CLV**, **Retention Rate %**, and **Repeat Purchase Rate** to move beyond basic reporting into behavioral analytics.

---


