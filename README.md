⚡ GANS Mobility Data Pipeline
Overview

GANS Mobility is a data-driven e-scooter company focused on optimizing fleet operations in major cities.
This project demonstrates how data engineering principles can be applied to automate the collection, processing, and storage of real-world information that influences scooter demand.

The pipeline integrates weather, flight, and demographic data, processes it using Python, and stores the results in a secure cloud database hosted on Google Cloud Platform (GCP).

Project Goal

The purpose of this project is to build an automated ETL (Extract, Transform, Load) system capable of gathering data from multiple public sources and turning it into actionable insights for mobility optimization.

The collected data supports strategic decisions such as where to deploy scooters, when to rebalance fleets, and how external factors like tourism or weather affect daily usage.

Architecture Overview

The system follows a modular workflow that moves data through several layers:

Data Collection – retrieves information from APIs and web sources

Data Cleaning & Transformation – standardizes formats and removes inconsistencies

Cloud Storage – stores processed data in a MySQL database on GCP

Automation – uses Google Cloud Functions and Scheduler to keep data up to date

Why Use the Cloud

Migrating to the cloud ensures scalability, continuous automation, and secure access for distributed teams.
GCP services handle storage, scheduling, and credentials, allowing the engineering focus to stay on building and improving data pipelines rather than maintaining infrastructure.

Tools & Technologies

Python 3 for data handling and scripting

pandas and JSON utilities for processing

MySQL (Google Cloud SQL) for structured storage

Google Cloud Functions for automation

Flask for local testing and debugging

Outcomes

By consolidating and automating data flows, GANS Mobility gains reliable insights into scooter usage trends and external influences such as weather or tourist arrivals.
The result is a scalable, maintainable, and cloud-ready data engineering solution built to grow with the company’s global operations.

Key Learnings

Designing modular ETL systems for flexibility and maintenance

Integrating multiple data sources into one coherent pipeline

Leveraging cloud infrastructure for automation and scalability

Applying Python for end-to-end data engineering workflows
