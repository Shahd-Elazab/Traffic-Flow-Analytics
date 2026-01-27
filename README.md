# 🚦 Traffic Flow Analytics

**End-to-End Data Engineering Project**

## 📌 Project Overview

Traffic Flow Analytics is a data engineering project developed as part of the **Digital Egypt Pioneers Initiative (DEPI)**.
The project focuses on building a complete data pipeline for traffic data, starting from data generation and streaming, through processing and storage, and ending with analytical visualization.

The system demonstrates how different data engineering components can be integrated to handle continuous data, organize it efficiently, and transform it into meaningful analytical insights.

---

## 🎯 Project Objectives

The main objectives of this project are to:

* Simulate continuous traffic data streams
* Stream data reliably using **Apache Kafka**
* Clean, preprocess, and transform data using **Apache Spark**
* Store data using a **layered Data Lake architecture**
* Model and analyze data using a **SQL Data Warehouse**
* Visualize insights through **Power BI dashboards**

---

## 🏗️ System Architecture

The project is organized into the following layers:

1. **Data Generation Layer**

   * Python scripts generate continuous traffic data (vehicle ID, speed, location, timestamp).
   * Data is streamed and also stored in CSV files for batch processing.

2. **Streaming Layer**

   * Apache Kafka is used to stream traffic data.
   * Configured with multiple brokers and partitions for reliability and parallelism.

3. **Preprocessing Layer**

   * Apache Spark processes raw CSV files.
   * Data is cleaned, grouped, and standardized.

4. **Data Lake Layer**

   * Data is stored in a structured Data Lake:

     * **Raw Zone**: Original generated data
     * **Processed Zone**: Cleaned and transformed data

5. **Data Warehouse Layer**

   * Processed data is loaded into **SQL Server**.
   * Analytical tables and transformations are applied.

6. **Visualization Layer**

   * Power BI dashboards provide insights such as:

     * Average and maximum speed
     * Vehicle count
     * Traffic distribution by location
     * Traffic trends over time

---

## 🧰 Technologies Used

* **Python**
* **Apache Kafka**
* **Apache Spark**
* **SQL Server**
* **Power BI**
* **Docker & Docker Compose**
* **CSV / Batch Processing**

---

## 📂 Project Structure

```
├── realtime_traffic_producer.py     # Traffic data generator & Kafka producer
├── traffic_generator_blob.py        # Data generation utilities
├── traffic_data.csv                 # Sample generated data
├── traffic_stream_analytics.ipynb   # Spark preprocessing and analytics
├── docker-compose.yml               # Kafka & service orchestration
├── requirements.txt                 # Python dependencies
├── Dashboard.pbix                   # Power BI dashboard
├── Project Documentation.pdf        # Detailed project documentation
```

---

## 👥 Team Contributions

This project was completed by a collaborative team, with each member responsible for a specific layer of the pipeline, including data generation, streaming, preprocessing, data lake design, data warehousing, and visualization.

---

## ✅ Key Features

* Continuous traffic data simulation
* Kafka-based streaming architecture
* Batch preprocessing using Apache Spark
* Layered Data Lake design
* SQL-based data modeling and analytics
* Interactive Power BI dashboards
* Modular and scalable pipeline structure

---

## 📊 Output

The final output of the project is an analytical dashboard that provides clear insights into traffic behavior, including speed patterns, vehicle distribution, and trends over time.

---

## 📎 Notes

This repository contains all scripts, configuration files, and documentation required to understand the project structure and workflow.

