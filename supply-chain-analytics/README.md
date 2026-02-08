# 📊 Logistics Performance & Revenue Risk Audit
**A Power BI Analytics Portfolio Project**

## 📖 Project Strategy
This project moves beyond standard reporting to provide a diagnostic audit of supply chain failures. By linking logistical latency to financial exposure, the dashboard enables stakeholders to prioritize interventions based on dollar value, not just shipment counts.

### 🎯 Business Objective
Identify the exact "where, who, and how much" of delivery delays to mitigate customer churn and safeguard **$13.69K in at-risk revenue**.

---

## 🛠️ Technical Deep-Dive

### 1. Data Architecture & ETL (Power Query)
The raw dataset required significant "cleaning" and restructuring to support multi-dimensional analysis:
* **Data Localization:** Performed metadata mapping to translate product categories from Portuguese to English, making the report accessible to international stakeholders.
* **Temporal Standardization:** Used locale-based conversion for DateTime fields to ensure accurate calculation of `Delay_Days` across different regional formats.
* **Star Schema Modeling:** Engineered a robust relationship model featuring role-playing dimensions for geography to independently track Seller and Customer locations.

### 2. The Analytics Engine (DAX)
I avoided basic counts in favor of "Strategic Measures" that drive action:
* **Revenue at Risk:** A high-impact calculation that filters total revenue by active delay flags.
* **Normalized Risk (Rate per 10K):** Created a fair comparison metric for geographic performance, removing the bias of population size in large states like SP.
* **Severity Buckets:** Transformed continuous delay data into categorical "Urgency Groups" (1-3 days, 4-7 days).

**Core Metric Logic:**
Revenue_At_Risk = CALCULATE([Total_Revenue], Fact_Shipments[Is_Delayed] = 1)

## 🧠 Overcoming Technical Challenges
•	The "Repetitive Chart" Problem: Initial drafts suffered from redundant bar charts. I solved this by implementing a Heatmap Matrix for root-cause analysis and a Scatter Chart to analyze the Correlation between Shipping Cost and Delivery Speed.

•	Relationship Complexity: Managing multiple date and location keys required a strict Star Schema approach to avoid circular dependencies and ensure high-speed filtering across all 4 dashboard pages.
________________________________________
## 📈 Executive Summary of Findings
🛑 Operational Root Causes

•	Node Failure: Warehouse 5 is the primary bottleneck in the network, particularly when routing through Dragonfly Express (1.19% delay rate).

•	Carrier Value: Loggi is identified as the "Gold Standard" for speed, while Correios contributes most to average delay severity.

💰 Financial & Regional Risk

•	Revenue Exposure: Health & Beauty products are the most financially vulnerable, with $3.70K currently delayed.

•	Geography of Risk: Geographic analysis reveals that customers in GO and ES face the highest probability of delay incidents.
________________________________________
## 🚀 Final Recommendations
1.	Contractual Review: Renegotiate SLAs with Dragonfly Express or re-route high-value shipments to Loggi.
2.	Process Audit: Conduct a deep-dive into Warehouse 5 internal fulfillment workflows.
3.	Retention Strategy: Proactively communicate with the Top 10 Sellers in the Health & Beauty category to manage customer expectations.
________________________________________
### 📊 The 16-Metric Analytics Framework
The dashboard's intelligence is powered by a tiered DAX architecture:

| Category | Metrics |
| :--- | :--- |
| **Volume** | Total Orders, Total Shipments, Total Customers |
| **Financial** | Total Revenue, Average Order Value (AOV) |
| **Performance** | On-Time Shipments, Delayed Orders, On-Time Delivery %, Delay Rate % |
| **Root Cause** | Avg Delay Days, Warehouse/Carrier/Seller Delay Rates |
| **Actionable** | Revenue at Risk, Delay Rate per 10K, Worst Carrier by Delay |

**Featured Logic (Revenue at Risk):**
Identifies the exact dollar value ($13.69K) of orders trapped in "Delayed" status, allowing for prioritized financial recovery.

## 📥 Power BI Dashboard File
[Download PBIX here](https://drive.google.com/file/d/12UYBHR4PYVsmSOd0UhZeUFCSgrFQkyI_/view?usp=sharing)


