# MovieLens Analytics with Databricks & PySpark

## 📌 Project Overview
This repository contains Big Data analysis on the MovieLens dataset using Databricks, Spark SQL, and PySpark DataFrames.

The project is split into two main notebooks:
1. **Exploratory SQL Analysis:** Loading raw CSV/pipe data into Delta tables and analyzing extreme rating categories (oldest highly-rated movies, popular low-rated movies).
2. **Polarizing Movies Analysis:** Identifying movies that split viewers (high number of 1-star AND 5-star ratings) using PySpark DataFrames & Spark SQL, including a custom normalization score.

## 📊 Key Findings
- **Pulp Fiction (1994)** ranks as the most polarizing movie in absolute volume (score: 209) and in normalized rate (53% extreme ratings).
- Standard popularity metrics skew polarization scores; normalizing by total ratings (`(1_star + 5_star) / total_ratings`) provides a more balanced metric.

## 🛠 Tech Stack
- **Platform:** Databricks (Unity Catalog)
- **Languages:** Python (PySpark), SQL
- **Storage Format:** CSV / Delta Lake
