# Project2_PySpark-Movie-Pipeline-Databricks-CE-

# 🎬 PySpark Movie Pipeline (Databricks CE)

## Overview
This project builds a **data pipeline using PySpark on Databricks CE** to process a movies dataset (IMDB-style).  
It demonstrates:
- Cleaning mixed date formats (`MM/dd/yyyy`, `dd-MM-yyyy`)
- Exploding multiple genres into separate rows
- Aggregating top genres and average ratings by year
- Saving results as **Parquet files** in DBFS
- Running SQL queries on Spark DataFrames

---

## Architecture
1. **Raw Data**: CSV uploaded into Databricks (`FileStore/movies/movies.csv`)
2. **Transformations**:
   - Parse mixed-format dates
   - Standardize schema (`title, genres, release_year, rating, country`)
   - Explode genres for multi-label analysis
3. **Aggregations**:
   - Top genres by count
   - Average rating by release year
4. **Output**: Saved results in Parquet (`/FileStore/movies/out/`)

---

## Pipeline (5 steps)

- **Cell 1**: Setup paths  
- **Cell 2**: Read CSV + clean schema  
- **Cell 3**: Explode genres  
- **Cell 4**: Aggregations  
- **Cell 5**: Save + query with SparkSQL  

---

## Sample Results
- **Top Genres by Count**  

- **Average Rating by Year**  

---

## Tech Stack
- PySpark (Databricks CE)  
- DBFS (Databricks File System)  
- SparkSQL  
- Python  

## Resume Line
“Built a PySpark pipeline in Databricks CE to process 50K+ movie records, parsing dates, exploding genres, and generating insights on top genres and ratings by year, with results saved as Parquet for analysis.”  
