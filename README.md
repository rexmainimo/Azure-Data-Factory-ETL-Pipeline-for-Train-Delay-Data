Author: Rex Mainimo   

Date: 27/06/2026

# Azure-Data-Factory-ETL-Pipeline-for-Train-Delay-Data
ETL pipeline using Azure Data Factory to ingest, transform, and export train operation data from Blob Storage. Includes filtering, delay calculations, and aggregations for reporting. Transformed data is stored back in Blob Storage for analysis.

## Project Overview

This project demonstrates the design and implementation of an ETL (Extract, Transform, Load) pipeline using **Azure Data Factory** to process train operation and delay data.

The pipeline ingests raw CSV files from Azure Blob Storage, applies data transformations, and outputs the cleaned and aggregated data back to Blob Storage. This processed data can be used for reporting, analysis, and visualization.

---

##  Features

- Ingests CSV data from Azure Blob Storage
- Data filtering to exclude invalid or incomplete records
- Derives new columns (e.g., total delay calculation)
- Aggregates delay data by train and relation
- Outputs final data to Blob Storage in a structured format (CSV or Parquet)
- Pipeline scheduling for daily automated runs

---

## 🛠 Technologies Used

- Azure Data Factory
- Azure Blob Storage
- CSV Data Format
- Basic Data Transformation (Filter, Derived Column, Aggregate)

---

## 📁 Dataset Columns

The dataset includes the following columns:

- `DATDEP`
- `TRAIN_NO`
- `RELATION`
- `TRAIN_SERV`
- `PTCAR_NO`
- `THOP1_COD`
- `LINE_NO_DEP`
- `REAL_TIME_ARR`
- `REAL_TIME_DEP`
- `PLANNED_TIME_ARR`
- `PLANNED_TIME_DEP`
- `DELAY_ARR`
- `DELAY_DEP`
- `CIRC_TYP`
- `RELATION_DIRECTION`
- `PTCAR_LG_NM_NL`
- `LINE_NO_ARR`
- `PLANNED_DATE_ARR`
- `PLANNED_DATE_DEP`
- `REAL_DATE_ARR`
- `REAL_DATE_DEP`

---

## 🚀 Getting Started

1. Provision Azure Data Factory and Azure Blob Storage (free student credits can be used)
2. Upload raw CSV files to your Blob Storage
3. Import this Data Factory pipeline into your Azure subscription
4. Configure linked services and datasets as required
5. Run or schedule the pipeline to process your data

---

## 📅 Future Improvements

- Integrate with Azure Synapse or Azure SQL Database for advanced reporting (optional)
- Add data validation steps
- Connect to Power BI for real-time dashboards

---

## 📄 License

This project is for educational purposes and is free to use under the [MIT License](LICENSE).
