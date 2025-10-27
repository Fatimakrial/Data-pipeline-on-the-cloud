# ⚡ GANS Mobility Data Pipeline

## Overview
**GANS Mobility** is a data-driven e-scooter company focused on optimizing fleet operations in major cities. This project demonstrates how data engineering principles can automate the collection, processing, and storage of real-world information that influences scooter demand.

The pipeline integrates weather, flight, and demographic data, processes it using Python, and stores the results in a secure cloud database hosted on **Google Cloud Platform (GCP)**.

---

## Project Goal
Build an automated **ETL (Extract, Transform, Load)** system that consolidates multiple public data sources into actionable insights for mobility optimization—informing where to deploy scooters, when to rebalance fleets, and how external factors (tourism, weather) affect usage.

---

## Architecture Overview
A modular workflow moves data through four layers:

1. **Data Collection** — retrieves information from APIs and web sources  
2. **Data Cleaning & Transformation** — standardizes formats and removes inconsistencies  
3. **Cloud Storage** — persists processed data in a MySQL database on GCP  
4. **Automation** — keeps data up to date via Google Cloud Functions and Scheduler

---

## Why Use the Cloud
Migrating to the cloud enables scalability, continuous automation, and secure access for distributed teams. GCP services handle storage, scheduling, and credentials so engineering effort can focus on building and improving pipelines rather than maintaining infrastructure.

---

## Tools & Technologies
- **Python 3** for data handling and scripting  
- **pandas** and JSON utilities for processing  
- **MySQL (Google Cloud SQL)** for structured storage  
- **Google Cloud Functions** for serverless automation  
- **Flask** for local testing and debugging

---

## Outcomes
By consolidating and automating data flows, **GANS Mobility** gains reliable insights into scooter usage trends and external influences such as weather or tourist arrivals. The result is a scalable, maintainable, and cloud-ready data engineering solution designed to grow with global operations.

---

## Key Learnings
- Designing modular ETL systems for flexibility and maintenance  
- Integrating multiple data sources into a unified pipeline  
- Leveraging cloud infrastructure for automation and scalability  
- Applying Python for end-to-end data engineering workflows
