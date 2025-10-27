⚡ GANS Mobility Data Pipeline
Overview

GANS Mobility is an e-scooter startup using data to optimize fleet distribution.
This project builds a cloud-based ETL pipeline that collects and processes external data — including weather, flights, and demographics — to support smarter scooter placement decisions.

The system runs automatically on Google Cloud Platform (GCP) and stores all processed data in a MySQL database.

🧭 Pipeline Summary
APIs & Web Sources
     ↓
Data Extraction (Python)
     ↓
Cleaning & Transformation (pandas)
     ↓
Cloud Storage (MySQL on GCP)
     ↓
Automation (Cloud Functions + Scheduler)


The modular structure allows independent testing and smooth deployment to GCP.

☁️ Why Cloud?

Automation: Regular data updates via Cloud Scheduler

Scalability: Handles growing data sources

Security: Managed access and credentials

Accessibility: Shared database for analytics and reporting

All functions can be tested locally with Flask before deployment.

🧰 Tools & Libraries
Purpose	Stack
Language	Python 3
Extraction	requests, BeautifulSoup, OpenWeather API
Processing	pandas, json, custom utils
Storage	MySQL (Google Cloud SQL)
Automation	Google Cloud Functions, Cloud Scheduler
Testing	Flask
📂 Project Structure
📁 gans-pipeline
├── cities.py          # City and country info
├── weather.py         # Weather data
├── flights.py         # Flight activity
├── demographics.py    # Population data
├── utils.py           # Helper functions
├── requirements.txt
└── README.md

⚙️ Setup
# Clone repo
git clone https://github.com/yourusername/gans-pipeline.git
cd gans-pipeline

# Install dependencies
pip install -r requirements.txt


Update credentials in utils.py:

RAPID_API_KEY = "your_key"
WEATHER_API_KEY = "your_key"
schema = "db_schema"
host = "gcp_host"
password = "password"


Run locally:

python cities.py
python weather.py
python flights.py


Deploy to Google Cloud:

@functions_framework.http
def main(request):
    # ETL process here
    return "Pipeline executed successfully"

📘 Key Takeaways

Built a scalable ETL pipeline using Python and GCP

Combined API and web-scraped data sources

Automated workflows with serverless cloud tools

Developed and tested locally with Flask
