# 🏥 Fabric-Healthcare-Analytics
> **End-to-end Data Engineering solution leveraging the Microsoft Fabric ecosystem to transform raw clinical data into actionable insights.**

---

## 🌟 Project Overview

This project demonstrates a production-grade data engineering lifecycle within the **Microsoft Fabric** environment. By applying the **Medallion Architecture**, I have engineered a pipeline that takes fragmented, simulated patient records and refines them into high-fidelity datasets for predictive analytics and facility reporting.

The primary focus is on **scalability**, **data integrity**, and **real-time accessibility**—critical factors in modern healthcare IT infrastructure.

---

## 🛠 Tech Stack & Tools

📊 **Microsoft Fabric** · 🔥 **Apache Spark** · 🐍 **Python** · 🗄️ **SQL** · ☁️ **Azure**

---

## 🏗 Medallion Architecture Plan

To ensure a robust system, the data flows through three distinct layers within **OneLake**:

| Layer | Status | Process |
|------|--------|---------|
| 🟫 **Bronze** | **Raw** | Ingestion of simulated JSON/CSV health records in their native format. |
| 🥈 **Silver** | **Validated** | Schema enforcement, deduplication, and PII (Personal Identifiable Information) masking using Spark. |
| 🥇 **Gold** | **Curated** | Business-level aggregates, such as *Patient Readmission Risk* and *Resource Utilization* metrics. |

---

## 🚀 Key Engineering Features

* **Orchestration:** Automated data movement using **Fabric Data Factory** pipelines.
* **Transformation:** High-performance data cleaning using **PySpark Notebooks**.
* **Storage:** Unified data storage in **Delta Lake** format for ACID compliance.
* **Intelligence:** Seamless integration with **Power BI** for real-time clinical dashboards.

---

## 📂 Project Structure

```text
├── 01-ingestion-bronze/   # Fabric Notebooks for data landing
├── 02-refinement-silver/  # Cleaning & validation logic
├── 03-analytics-gold/     # Aggregation & Gold layer views
├── data/                  # Sample synthetic datasets
└── docs/                  # Architecture diagrams and documentation
