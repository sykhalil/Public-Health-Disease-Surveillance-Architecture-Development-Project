# Public-Health-Disease-Surveillance-Architecture-Development-Project
Synthetic Healthcare Data Pipeline for COVID-19 Surveillance and Reporting

# Architecture Development Part 6  
## Aggregation and Visualization of Data for Disease Outbreak Surveillance

## Overview

This project demonstrates the development of a healthcare data analytics pipeline for disease outbreak surveillance using synthetic patient records generated with **Synthea**. Data from four simulated hospitals was aggregated, transformed, analyzed, and visualized to simulate how public health agencies can monitor infectious disease trends in near real time.

Using Python and data processing tools, FHIR-based `.json` patient files were converted into structured CSV datasets. COVID-19 related cases were then analyzed and presented through an interactive dashboard built in **Google Looker Studio**. link to report : https://datastudio.google.com/reporting/1e6585a6-320a-41ef-814b-57cc747c6c7a

---

# Project Objectives

The primary objectives of this project were:

- Aggregate healthcare data from multiple hospitals into a unified dataset  
- Understand and work with FHIR-based healthcare JSON records  
- Identify and analyze COVID-19 related cases using synthetic patient data  
- Convert raw healthcare records into clean CSV datasets  
- Build a public health dashboard for outbreak surveillance  
- Visualize geographic and city-based disease distribution  
- Simulate real-world healthcare analytics workflows using privacy-safe synthetic data  

---

# Technologies Used

This project used the following tools and technologies:

### Programming & Data Processing
- Python  
- Pandas  
- Jupyter Notebook  
- JSON Parsing  
- CSV Data Transformation  

### Healthcare Data Standards
- FHIR (Fast Healthcare Interoperability Resources)  
- Synthea Synthetic Patient Generator  

### Business Intelligence & Visualization
- Google Looker Studio  
- Geographic Mapping  
- Dashboard Analytics  

### Environment
- Ubuntu Linux (WSL)  
- VS Code / Jupyter Environment  

---

# Why This Project Matters

Healthcare organizations rely on data systems like this to:

- Detect disease outbreaks early  
- Track case distribution geographically  
- Improve decision-making for hospitals and agencies  
- Allocate resources efficiently  
- Increase public awareness through dashboards  
- Support evidence-based health policy decisions  

---

# Data Sources

Synthetic healthcare data was generated from four simulated hospitals:

- MGH  
- PortageHealth  
- BCMH  
- Aspirus  

Each hospital contained exported FHIR-based patient `.json` files representing realistic healthcare records without exposing private information.

---

# Methodology

## Step 1: Data Aggregation

Patient files from all hospitals were processed using Python scripts to extract structured healthcare data.

Generated outputs included:

- Patient.csv  
- Observation.csv  
- Encounter.csv  
- Condition.csv  
- CarePlan.csv  

## Step 2: COVID-19 Investigation

COVID-related diagnosis codes were isolated and analyzed.

Additional processed outputs:

- covid_final_clean.csv  
- covid_dashboard.csv  

## Step 3: Dashboard Reporting

The final CSV data was connected to Google Looker Studio to build an outbreak surveillance dashboard featuring:

- Geographic map of cases by city  
- Bar chart of cases by city  
- Auto-refresh every 15 minutes  
- Interactive filtering  

---

# Challenges Faced

Several technical and analytical challenges were addressed during this project:

### Complex Healthcare JSON Structure
FHIR records contain nested and interconnected fields that required careful parsing and transformation.

### Large Data Processing Load
Processing many `.json` files across four hospitals required RAM awareness and efficient scripting.

### Data Cleaning
Records needed filtering, merging, and standardization before meaningful analysis.

### COVID Code Identification
Accurately isolating COVID-19 related conditions required understanding diagnosis coding structures.

### Dashboard Preparation
Raw outputs had to be reshaped into dashboard-friendly CSV files suitable for Looker Studio.

### Geographic Visualization Setup
Location fields needed proper formatting for successful mapping and charting.

---

# Outcomes Achieved

This project successfully produced the following outcomes:

### Functional Data Pipeline
Built a working end-to-end pipeline from raw patient JSON files to analytics dashboard.

### Multi-Hospital Aggregation
Combined healthcare data from four simulated hospitals into unified datasets.

### COVID Surveillance Analytics
Generated city-level COVID case insights and comparative metrics.

### Interactive Dashboard
Created a publicly shareable Looker Studio dashboard for outbreak monitoring.

### Real-Time Reporting Simulation
Configured dashboard refresh cycles every 15 minutes.

### Practical Experience
Developed hands-on skills in healthcare analytics, ETL pipelines, BI tools, and public health reporting.

---

# Repository Structure

```text
Architecture_Development_Part6/
│── notebooks/
│   ├── Synthea_Patient_Data_Aggregation_Util_SuhaKhalil.ipynb
│   └── SuhaKhalil_BonusAssignment.ipynb
│
│── hospital_data/ (Not added to Repository due to huge data size)
│   ├── MGH/
│   ├── PortageHealth/
│   ├── BCMH/
│   ├── Aspirus/
│   └── output/
│       ├── Patient.csv
│       ├── Observation.csv
│       ├── Encounter.csv
│       ├── Condition.csv
│       └── CarePlan.csv
│
│── Suha's Code outputs/
│   ├── covid_final_clean.csv
│   └── covid_dashboard.csv
│
│── dashboard/
│   └── Looker_Studio_Report_Link.txt
│
└── README.md
---
