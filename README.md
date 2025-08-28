# 📊 Fraud Procurement Analysis – Power BI Project  

## 🔹 Objective  
The primary objective of this project is to **detect and monitor procurement fraud patterns** by analyzing vendor transactions, purchase orders, invoice data, and approval workflows. The solution helps identify **suspicious vendors, duplicate invoices, dependency risks, and mismatches** in procurement data.  

---

## 🔹 Purpose  
- To showcase the application of **Data Analytics in Procurement Fraud Detection**.  
- To build a **Power BI dashboard** that provides business users and auditors with actionable insights.  
- To use **synthetic procurement data** (since real-world sensitive procurement data is not available) that mimics realistic fraud scenarios.  

---

## 🔹 Data  
- **Synthetic Dataset Creation**  
  - Data tables were generated to simulate real procurement workflows.  
  - Fact & Dimension tables include:  
    - `Fact_Procurement` – Purchase Order IDs, Vendor IDs, Approvers, PO Amounts, Invoice Amounts, Risk Flags, etc.  
    - `Dim_Vendor` – Vendor details, risk category.  
    - `Dim_Category` – Procurement categories.  
    - `Dim_Approver` – Approver details.
    - 'Dim_Date' - Date Range 
  - Fraud-related features were introduced:
    - **Duplicate invoices**  
    - **Vendor dependency (High/Medium/Low)**  
    - **Mismatch between PO Amount & Invoice Amount**  
    - **High-Risk Vendor flag**  

---

## 🔹 Approach  
1. **Data Preparation**  
   - Created synthetic data in Excel/CSV using Python.  
   - Cleaned and modeled the data in Power BI (Star Schema).  

2. **Data Modeling**  
   - Relationship setup between Fact & Dimension tables.  
   - Added calculated columns and DAX measures for fraud metrics.  

3. **Dashboard Design**  
   - Multiple report pages were created to cover procurement fraud insights:  
     - **Procurement Overview** – Spend summary, PO trends, vendor distribution.  
     - **Vendor Risk Analysis** – High-risk vendors, dependency risks.  
     - **Category & Approver Insights** – Approver patterns, category-level risks.  
     - **Invoice Quality** – Duplicate invoices, mismatch analysis.  
     - **Fraud Monitor** – Detailed table of suspicious transactions with drill-through capability.  
     - **Trends & QoL** – Historical procurement trends, quality-of-life indicators for audit teams.  
     - **Risk Actions & Recommendations** – Suggested follow-up actions and data-driven recommendations for fraud cases.  

---

## 🔹 Key Metrics (DAX Measures)  
- **Risk Cases** = COUNT of transactions with Risk_Flag.  
- **Risk %** = Risk Cases ÷ Total Transactions.  
- **Vendor Dependency Rate** (Low/Medium/High).  
- **Duplicate Invoice Count**.  
- **Mismatch Rate** between PO & Invoice.  
- **Trend Measures** – Year-over-Year growth in suspicious POs, risk % changes over time.  

---

## 🔹 Outcome  
- A **Fraud Procurement Dashboard** that:  
  - Flags **suspicious vendors & invoices**.  
  - Helps identify **approver anomalies**.  
  - Provides **risk trends and QoL indicators** for monitoring.  
  - Suggests **risk actions and recommendations** to minimize fraud.  
- Demonstrates how **data-driven insights** can reduce procurement risks and improve audit efficiency.  

---

## 🔹 Tools & Technologies  
- **Power BI** – Dashboarding, Data Modeling, DAX.  
- **Excel/CSV** – Synthetic data generation.  
- **GitHub** – Version control & sharing.  

---

## 🔹 How to Use  
1. Clone this repository:  
   ```bash
   git clone https://github.com/your-username/fraud-procurement-powerbi.git

