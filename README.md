# Customer Demographics & Sales Analytics Pipeline (Azure Data Engineering Project)

## 📌 Project Overview
This project implements an **end-to-end data engineering pipeline** for an E-commerce dataset using the **Azure Data Engineering Stack**.  
The pipeline ingests raw transactional and customer data, transforms it using the **Medallion Architecture (Bronze → Silver → Gold)**, and stores it in **Azure Synapse** for reporting and analytics.  

The solution provides stakeholders with **insights into sales performance, customer demographics, and product trends** via fact and dimension tables, which can be visualized in Power BI.

---

## 🏗️ Architecture
- **Azure Data Factory (ADF):** Data ingestion and orchestration from raw sources.  
- **Azure Data Lake Storage (ADLS Gen2):** Centralized storage for raw (Bronze), cleansed (Silver), and aggregated (Gold) data.  
- **Azure Databricks:** Data cleaning, transformation, and processing using PySpark and Delta Lake.  
- **Azure Synapse Analytics:** Data warehouse for structured storage, SQL-based queries, and BI integration.  
- **Power BI (Optional):** For data visualization and dashboard creation.  

---

## 🔄 Workflow
1. **Data Ingestion:** Load raw e-commerce data (transactions, customers, products) into **ADLS Bronze** using ADF.  
2. **Data Transformation:** Use **Databricks notebooks** to clean, standardize, and enrich data → move to **Silver**.  
3. **Data Modeling:** Create **Fact & Dimension tables** in the **Gold layer** for analytical queries.  
4. **Data Loading:** Store processed data in **Azure Synapse** for BI and reporting.  
5. **Visualization:** Build **Power BI dashboards** for sales performance and customer insights.  

---

## 🛠️ Tech Stack
- **Azure Data Factory** – Data ingestion & orchestration  
- **Azure Data Lake Gen2** – Centralized storage (Bronze, Silver, Gold)  
- **Azure Databricks (PySpark, Delta Lake)** – Data transformation  
- **Azure Synapse Analytics** – Data warehousing  
- **Power BI** – Dashboard and reporting  

---

## 📊 Key Business Outcomes
- Centralized **sales and customer analytics** pipeline for E-commerce data.  
- Reduced manual reporting through **automated ETL workflows**.  
- Enabled business teams to analyze **trends in sales, product performance, and customer demographics**.  

---

## 📂 Repository Structure
```

├── data/
│   ├── raw/        # Raw e-commerce data
│   ├── bronze/     # Parquet files (source of truth)
│   ├── silver/     # Cleaned, enriched data
│   ├── gold/       # Fact & Dimension tables
├── notebooks/
│   ├── ingestion/
│   ├── transformations/
│   ├── modeling/
├── reports/
│   ├── dashboards/

```

---

## 🚀 Future Enhancements
- Add **real-time ingestion** using Event Hubs/Stream Analytics.  
- Implement **CI/CD for ADF & Databricks pipelines**.  
- Extend to **predictive analytics (customer churn, product recommendation)**.  
```
