# Module 22 - SparkSQL-challenge: Home Sales Analysis
---
## Objectives

- Read and process a CSV dataset from AWS S3 to a PySpark DataFrame.
- Create and manage temporary tables for SQL querying.
- Analyze average home prices using different filters/attributes.
- Compare performance between uncached, cached, and partitioned Parquet data queries.

---

## Tools Used

- Apache Spark (PySpark)
- Google Colab/Jupyter Notebook
- AWS S3 as data source
- Parquet file format
- SQL (Spark SQL)

---

## Key Analysis Steps

1. **Data Loading**: Load CSV data directly from AWS S3 into a Spark DataFrame.
2. **Temporary Views**: Create SQL-accessible views for querying the dataset.
3. **SQL Analysis**:
   - Average price for 4-bedroom homes sold each year
   - Average price for 3 bed / 3 bath homes by year built
   - Average price for 3 bed / 3 bath / 2 floor / ≥2000 sqft homes
   - Average price per view rating ≥ $350,000 (with runtime measurement)
4. **Caching and Performance**:
   - Cached query execution vs. uncached
   - Save partitioned Parquet data by `date_built`
   - Query Parquet view and compare runtime
5. **Cleanup**:
   - Uncache and verify memory cleanup of the Spark table

---

## Resources

Relied on in class activites and examples from the instructor i.e. curriculum content.
ChatGPT was used for conceptual support, as well as, for clarity with data analysis.
