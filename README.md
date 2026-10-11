# 💳 Credit Card Financial & Customer Analytics Dashboard

## 📌 Project Overview
An end-to-end business intelligence solution developed to analyze credit card transaction operations and customer demographic behavior. The project transforms raw financial transaction data into interactive analytical reports to track revenue performance, payment channel usage, portfolio risk, and customer segmentation.

---

## 🛠️ Data Pipeline & Technical Architecture

1. **Data Preprocessing (Microsoft Excel):** Cleaned, inspected, and prepped initial transaction and customer datasets.
2. **Database Management (PostgreSQL):** Designed the relational schema and loaded preprocessed CSV files into dedicated database tables.
3. **Data Modeling & DAX Engineering (Power BI):**
   * Engineered a calculated **`Revenue`** column in the `credit_card` table to track transaction earnings[cite: 12].
   * Created **`AgeGroup`** and **`IncomeGroup`** conditional DAX columns in the `customer` table to enable demographic segmentation[cite: 14].
   * Established table relationships on `Client_Num` to enable cross-filtering across transaction and customer dimensions[cite: 12, 14].

---

## 📊 Dashboard Modules & Analysis

### 1. Credit Card Transaction Report
Focuses on operational financial health, card tiers, payment channels, and temporal spend trends:
* **Revenue by Card Category:** Donut chart evaluating revenue distribution across tiers (Blue, Silver, Gold, Platinum), showing Blue cards driving the majority share (83.4%)[cite: 11].
* **Payment Modes by Transaction Amount:** Donut visual analyzing payment channel preferences across **Swipe** (69.59%), **Chip** (24.69%), and **Online** (5.72%)[cite: 11].
* **Weekly Revenue Trends:** Column visual tracking chronological performance fluctuations over continuous billing cycles[cite: 11].
* **Expenditure Categories:** Bar chart categorizing spend across essential and discretionary buckets (**Bills**, **Entertainment**, **Fuel**, **Grocery**, **Food**, **Travel**)[cite: 11].
* **Summary Matrix:** Tabular breakdown displaying revenue, transaction amounts, interest earned, and customer acquisition costs per card type[cite: 11].

### 2. Customer Demographics Report
Focuses on cardholder segmentation, risk profiles, and behavioral metrics:
* **Executive KPI Cards:** Immediate tracking of **Average Customer Age (46.25)**, **Total Customer Base (5.39K)**, and **Customer Satisfaction Score (3.19 / 5.0)**[cite: 13].
* **Job Classification Breakdown:** Horizontal bar chart profiling client distribution across professions, identifying **Self-employed** and **Business** professionals as the largest segments[cite: 13].
* **Income Segmentation:** Donut chart illustrating balanced portfolio adoption across **Low (38.5%)**, **Medium (31.4%)**, and **High (30.1%)** income brackets[cite: 13].
* **Age Distribution:** Column visual illustrating customer volume concentration, peaking heavily in the **40–50** age cohort followed by **50–60**[cite: 13].
* **Education & Marital Status:** Cross-demographic analysis showing household makeup and graduation status across cardholders[cite: 13].
* **Interactive Slicers:** Dynamic filtering by State code (`state_cd`) and Home Ownership (`House_Owner`)[cite: 13].

---

## 📈 Key Business Insights

* **Dominant Spend Channel:** Physical card interactions dominate usage, with **Swipe transactions** accounting for nearly **70%** of total transaction volume[cite: 11].
* **Essential Spend Bias:** Routine household overhead (**Bills at 14M**, **Fuel**, and **Groceries**) outpaces discretionary categories like **Travel ($1.5M)**[cite: 11].
* **Primary Demographics:** The core user base is concentrated in middle-aged cohorts (**40–50 years**, average age **46.25**), with minimal penetration in the 20–30 bracket[cite: 13].
* **Customer Base Distribution:** Balanced representation across income brackets indicates strong product utility across both mass-market and affluent tiers[cite: 13].

---

## 💻 Tech Stack & Skills Demonstrated
* **Database & Querying:** PostgreSQL (Schema Setup, Data Ingestion, Relational Tables)
* **Data Prep:** Microsoft Excel (Data Cleansing & Validation)
* **BI & Analytics:** Power BI Desktop (Data Modeling, DAX, Custom Measures, Calculated Columns)
* **Core Competencies:** Business Intelligence (BI), KPI Tracking, Financial Analytics, Customer Segmentation, Data Visualization
