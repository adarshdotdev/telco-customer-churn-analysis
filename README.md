# 📊 Telco Customer Churn Analysis

This project analyzes a telecom customer dataset to understand the reasons behind customer churn and identify the key factors influencing it. The analysis is aimed at supporting data-driven decisions to reduce churn and improve customer retention strategies.

---

## 🧠 Executive Summary

- **Churn Rate:** 26.54% of customers have left the service  
- **Goal:** Identify what drives churn and suggest retention strategies  
- **Tools Used:** Python, Pandas, Matplotlib, Seaborn, Jupyter Notebook  

---

## 🔧 Data Preparation

- Loaded and cleaned `telco-customer-churn-data.csv`
- Replaced blank values in `TotalCharges` with 0 and converted the column to numeric
- Encoded `SeniorCitizen` to `"Yes"` and `"No"` for clarity
- Verified no nulls or duplicates in key fields

---

## 📉 Churn Distribution

- **26.54%** customers have churned  
- Indicates a high churn rate and potential service or satisfaction issues

---

## 🔍 Key Drivers of Churn

### 1. Gender  
- Churn rate is similar for both genders  
- **No significant impact** from gender

### 2. Senior Citizens  
- Senior citizens have a **higher churn rate**  
- Count plots clearly show this trend

### 3. Tenure  
- **< 5 months:** very high churn  
- **> 1 year:** significantly lower churn  
- Early retention efforts are **critical**

### 4. Contract Type  
- **Month-to-month:** ~43% churn  
- **One-year:** ~11% churn  
- **Two-year:** ~3.8% churn  
- **Insight:** Long-term contracts = better retention

### 5. Internet & Streaming Services  
- **Fiber Optic** users churn more than DSL/No Internet  
- Customers **without security, tech support, or device protection** churn more  
- Users **not using streaming services** churn less

### 6. Phone Service  
- No major churn difference based on Phone Service  
- Slightly higher churn among those with **Multiple Lines**

---

## 🧠 Insights Summary

| Feature          | Insight                                  |
|------------------|-------------------------------------------|
| Churn Rate       | 26.54%                                    |
| Tenure           | <5 months = high churn; >12 months = low churn |
| Contract Type    | Month-to-month = 43% churn; 2-year = 3.8% |
| Senior Citizens  | More likely to churn                     |
| Internet Type    | Fiber Optic users churn more             |
| Add-on Services  | No tech support/security = higher churn  |

---

## ✅ Recommendations

- Offer **longer contracts** with bundles or discounts  
- Focus on **early retention** in the first 3–6 months  
- Improve **tech support and add-on services** value  
- Reassess **Fiber Optic** service satisfaction and experience

---

## 📁 Files Included

```bash
.
├── telco_churn_analysis.ipynb       # Full analysis notebook
├── telco-customer-churn-data.csv    # Dataset
└── summary_report.pdf               # Executive summary report
