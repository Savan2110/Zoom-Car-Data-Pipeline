# 🚗 ZoomCar Data Processing Pipeline

A data engineering project built with **Databricks, PySpark, and Delta Lake** to process ZoomCar’s customer and booking data.  
This project demonstrates an **end-to-end ETL pipeline** including ingestion, transformation, and loading into target tables for analytics.

---

## 📸 Project Snapshots
*(Upload your screenshots in the `images/` folder and replace below placeholders)*  

- ![Pipeline Architecture](<img width="1677" height="937" alt="pipeline" src="https://github.com/user-attachments/assets/d1dfac71-5b06-4632-8ae5-45be2d614c37" />)  
- ![Databricks Workflow](<img width="1677" height="930" alt="job_run" src="https://github.com/user-attachments/assets/1b166b9c-0fdc-4965-958f-8b16aa73ef8e" />)  
- ![Delta Table Output](<img width="1680" height="858" alt="target_bookings_delta" src="https://github.com/user-attachments/assets/7202eb11-b4b8-4c36-8feb-722bbf420f53" /><img width="1677" height="897" alt="target_customers_delta" src="https://github.com/user-attachments/assets/2d9dca97-e725-4f2e-91dc-8ce0609c2525" />)  

---

## 🔍 Overview

This pipeline processes raw JSON booking and customer data from ZoomCar into clean, optimized Delta tables ready for analytics.  

Key highlights:
- Raw data ingestion from JSON files (simulated as if coming from ADLS/Blob storage).
- Data cleaning and standardization with PySpark.
- **Delta Lake merge operations** to handle inserts, updates, and deletes (SCD-Type 2 style).
- Automated execution using **Databricks Jobs & Workflows**.
- Organized repository for reproducibility.

---

## 🧰 Tech Stack

- **Databricks** → notebook-based development & orchestration  
- **PySpark** → distributed data processing  
- **Delta Lake** → ACID-compliant data storage  
- **Azure Data Lake Storage (ADLS)** → raw & processed data layers  

---

## 📂 Repository Structure

```plaintext
zoom-car-data-pipeline/
├── data/              # sample or raw input files
│   └── raw/
├── notebooks/         # exported Databricks notebooks
│   ├── customers.ipynb
│   ├── bookings.ipynb
│   └── merge.ipynb
├── src/               # optional reusable PySpark scripts
├── images/            # screenshots (pipeline, jobs, outputs)
├── requirements.txt   # dependencies
├── .gitignore
├── LICENSE
└── README.md
