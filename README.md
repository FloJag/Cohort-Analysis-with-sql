# 📊 Cohort Analysis – Sales Dataset

This project performs a cohort analysis based on a sales dataset. The goal is to analyze the behavior of different customer groups (cohorts) over time — particularly regarding retention, revenue trends, and repeat purchases.

## 🚀 Project Overview

The repository includes:

- **Transformation Queries** – SQL queries for preparing and segmenting raw data  
- **Visuals Queries** – SQL queries to generate aggregated metrics for visualizations  
- **Dashboard** – Visualizations (e.g., Tableau / PowerBI / Notebook) presenting the results  
- **Presentation** – Presentation materials explaining the key insights  
- **Notebook(s)** – Exploratory analysis (if available)  

The project analyzes a total of 6 cohorts, created based on a defined criterion (e.g., first purchase month).

## 🧠 What is Cohort Analysis?

Cohort analysis groups users or customers based on a shared characteristic — for example, the time of their first purchase — and tracks their behavior over subsequent periods.

### Example Questions:

- How does customer retention evolve per cohort?  
- Which cohorts show high repeat purchase rates?  
- How does revenue change across different time periods for a cohort?  
- What actions could improve retention?

## 🏗️ Architecture (Medallion Architecture)

The presentation describes an end-to-end data pipeline for analysis, based on the Medallion Architecture.

### Data Pipeline Steps

1. **Data Source → BigQuery Upload**  
   Raw data is collected and uploaded to BigQuery.

2. **Connector**  
   Establishing the connection between the dataset in BigQuery and Databricks

3. **Delta Lake → Ingestion in Databricks**  
   Data is ingested into Databricks for reliable storage and processing.
   
5. **Transformation**  
   SQL queries are used to clean, prepare, and structure the data for analysis.

6. **Visuals**  
   Visualization of cohort behavior based on the transformed dataset.

## 💡 Insights 

The main findings from the cohort analysis:

- **Cohort sizes vary greatly**  
  There is significant variation in the number of customers per cohort.

- **Retention rate increases as the year goes on**  
  Later cohorts show improved retention over time.

- **Cohort 6:** All customers repurchased within the first month  

- **Cohorts 1–3:** Strongest purchasing power (frequency)  

- **Cohorts 1–2:** Buy more frequently, but require more time before making their next purchase  

**Attention:** Cohort size influences variability in customer behavior within a cohort. 

## 🏁 Conclusion
Cohorts 1 and 2 exhibit similar purchasing behavior, while cohorts 3–6 differ significantly in comparison.


