# Automated Twitter Data ETL Pipeline using Apache Airflow

## 📌 Project Overview

This project implements an **automated data engineering pipeline** that extracts data from the **Twitter (X) API**, processes it using **Python-based ETL logic**, and orchestrates the workflow using **Apache Airflow**. The pipeline is designed to run on a schedule, ensuring reliable, repeatable, and fault-tolerant data ingestion suitable for analytics and downstream processing.

---

## 🏗️ Architecture

1. **Twitter API** – Source of raw social media data
2. **Python ETL Scripts** – Data extraction, cleaning, and transformation
3. **Apache Airflow** – Workflow orchestration using DAGs
4. **Storage Layer** – Structured data stored locally or in cloud storage (Azure Data Lake / Blob Storage – optional)

---

## ⚙️ Technologies Used

* **Programming Language:** Python
* **Workflow Orchestration:** Apache Airflow
* **Data Ingestion:** Twitter API
* **ETL Processing:** Python
* **Scheduling & Automation:** Airflow DAGs
* **Version Control:** Git, GitHub
* **Optional Cloud Storage:** Azure Data Lake Gen2 / Azure Blob Storage

---

## 📂 Project Structure

```
twitter-airflow-data-engineering-project/
│── README.md
│── twitter_dag.py          # Airflow DAG definition
│── twitter_etl.py          # ETL logic for data extraction & processing
│── twitter_commands.sh     # Helper shell commands
```

---

## 🚀 Features

* Automated extraction of Twitter data using APIs
* End-to-end ETL pipeline orchestrated with Apache Airflow
* Scheduled DAG execution with task dependencies
* Fault tolerance using retries and logging
* Analytics-ready structured data output

---

## ▶️ How to Run the Project

### 1️⃣ Prerequisites

* Python 3.8+
* Apache Airflow installed
* Twitter Developer API credentials

### 2️⃣ Setup Virtual Environment

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### 3️⃣ Configure Airflow

```bash
airflow db init
airflow users create \
  --username admin \
  --password admin \
  --firstname Admin \
  --lastname User \
  --role Admin \
  --email admin@example.com
```

### 4️⃣ Start Airflow

```bash
airflow webserver
airflow scheduler
```

### 5️⃣ Trigger DAG

* Open Airflow UI: `http://localhost:8080`
* Enable and trigger the **Twitter Data ETL DAG**

---

## 📊 Output

* Extracted and transformed Twitter data stored in structured format
* Ready for analytics, reporting, or further processing

---

## 🔮 Future Enhancements

* Store data directly in **Azure Data Lake Gen2**
* Integrate **Azure Synapse Analytics** for querying
* Add data quality checks and monitoring
* Extend pipeline for real-time streaming ingestion

---

## 👤 Author

**Zaid Ali**
Aspiring Software Developer 

---

⭐ If you find this project useful, feel free to star the repository!
