# 📊 Telco Customer Churn – Business Intelligence Solution

A complete BI project built for customer churn analysis in the telecom industry, using **ETL**, **OLAP cube**, **Power BI**, **Excel Pivot**, and **Data Mining** to support decision-making and business strategies.

---

## 🔍 Project Overview

This project analyzes customer churn behavior using a Telco dataset (from Kaggle) and provides insights for different business units (retention, pricing, operations, etc.) through:

- **Data Warehouse (Star Schema)**
- **SSIS ETL process**
- **SSAS OLAP Cube with MDX**
- **Power BI dashboards & Excel pivot tables**
- **Churn prediction models** using machine learning

---

## 🏗️ Tech Stack

- **SQL Server Integration Services (SSIS)** – ETL pipeline  
- **SQL Server Analysis Services (SSAS)** – OLAP cube  
- **Power BI & Excel** – Data visualization  
- **Python (scikit-learn, XGBoost, CatBoost)** – Churn prediction  
- **Microsoft SQL Server** – Data warehouse  

---

## 🧱 Data Warehouse Schema

- **Fact Table**: `CustomerChurnFact`
- **Dimensions**:
  - `Dim_Customer`
  - `Dim_InternetService`
  - `Dim_PaymentMethod`
  - `Dim_AdditionalServices`
  - `Dim_Contract`
  - `Dim_Tenure`
  - `Dim_Churn`

📐 **Schema Type**: Star schema

---

## 📈 Business Intelligence Scenarios

| #  | Scenario                                  | Chart Type             | Business Use                  |
|----|-------------------------------------------|-------------------------|-------------------------------|
| 1  | TenureGroup × Churn                       | Stacked Column Chart    | Loyalty campaign              |
| 2  | InternetService × ContractGroup           | Clustered Bar Chart     | Pricing discounts             |
| 3  | PaymentCategory × PaperlessBilling        | Treemap                 | Revenue & paperless strategy  |
| 4  | Contract × InternetAvailability           | Grouped Column Chart    | Service upgrade campaign      |
| 5  | TenureRange × SeniorCitizen               | Box Plot                | Senior-focused packages       |
| 6  | InternetService × Dependents              | Line Chart              | Single customer retention     |
| 7  | PaymentMethod × Churn                     | Pie/Bar Chart           | Promote auto-pay              |
| 8  | ContractGroup × Gender                    | Stacked Bar Chart       | Gender-targeted promotions    |
| 9  | Tenure × Partner                          | Line Chart              | Family loyalty program        |
| 10 | InternetService × PaperlessBilling        | Grouped Bar Chart       | Green billing campaign        |

Each of these is implemented using **SSAS cubes, MDX queries, Power BI visuals**, and **Excel pivots**.

---

## 🤖 Data Mining & Churn Prediction

We implemented and compared **6 machine learning models** to predict churn:

- Logistic Regression  
- Random Forest  
- Gradient Boosting  
- XGBoost  
- CatBoost  
- Neural Network (ANN)

**📌 Best models**: Logistic Regression, Gradient Boosting, CatBoost  
**📈 Evaluation**: ROC AUC, Confusion Matrix, Feature Importance

---

## 💡 Key Insights

**Most important features**:
- Contract type
- Tenure
- MonthlyCharges

**Customers with:**
- Month-to-month contracts  
- High monthly charges  
- Short tenure  
→ Have a **high risk of churn**

---

## 📌 Key Business Rules (from classification)

- Customers on **month-to-month contracts**, with **low tenure**, and **high monthly charges** are most likely to churn.
- Customers on **1–2 year contracts** are less likely to churn regardless of charge amount.
- Promoting **automatic payments**, **bundled services**, and **long-term contracts** can **effectively reduce churn**.

---
