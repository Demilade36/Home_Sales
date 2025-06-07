# Home Sales SparkSQL Analysis

This project uses **PySpark** and **SparkSQL** to analyze home sales data stored in an AWS S3 bucket. The analysis answers key business questions about average home prices based on bedroom count, year built, view rating, and other criteria. Performance optimization techniques like **caching**, **partitioning**, and **parquet formatting** are also applied and evaluated.

---

## Objectives

- Read a CSV dataset from AWS S3 using PySpark.
- Register a temporary SQL table.
- Use SparkSQL to run multiple queries involving filters, grouping, and aggregation.
- Cache data to improve query performance and compare execution times.
- Partition and save data in Parquet format to further optimize performance.
- Measure query execution times and interpret the results.

---

## Files

- `Home_Sales.ipynb` – Final Jupyter Notebook containing all completed tasks and queries.
- `home_sales_revised.csv` – Source data from AWS S3.
- `README.md` – Project overview and documentation (this file).

---

## Technologies

- Google Colab (Jupyter Notebook)
- Apache Spark (via PySpark)
- SparkSQL
- AWS S3
- Parquet

---

## Tasks & Deliverables

### 1. Data Import & Preparation
- Imported PySpark SQL functions.
- Loaded `home_sales_revised.csv` from AWS S3 into a Spark DataFrame.
- Created a temporary SQL table: `home_sales`.

### 2. SQL Queries
- Perform four queries
- One Uncached query runtime 

### 3. Optimization Techniques
- Caching.
- Reran the query on cached data and compared execution time.
- Partitioning & Parquet
- Uncache

---

## Performance Comparison

| **Scenario**                 | **Query Runtime (Approx.)**             |
|-----------------------------|------------------------------------------|
| Uncached query              | 0.89 seconds                             |
| Cached query (first run)    | 2.02 seconds *(due to caching overhead)* |
| Partitioned Parquet         | 1.32 seconds *(Faster than Cached)*      |

---

## 📌 Summary

This project demonstrates how **PySpark** and **SparkSQL** can be used to perform **scalable** and **efficient data analysis**. By implementing performance enhancements like **caching** and **partitioning**, we explored how **Big Data tools** optimize operations for **real-time analytics**.  
All analysis was completed in **Google Colab** using **PySpark**, enabling rapid prototyping in a cloud-based environment.

