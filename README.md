# soc-log-analysis-python-splunk
Beginner SOC project analysing Linux logs manually, automating detection with Python, and visualising suspicious activity in Splunk.

# Linux Log Analysis, Python Automation & SIEM Visualisation with Splunk

## Project Overview

This beginner SOC-level project focuses on analysing Linux system logs, automating suspicious activity detection with Python, and visualising security events in Splunk Enterprise.

The project was completed as part of Sandra Liu’s course and helped me understand how SOC analysts move from raw log data to detection, triage, and security insights.

---

## Objectives

### 1. Manual Linux Log Analysis
- Reviewed a Linux log dataset containing approximately 2,000 log entries.
- Analysed the logs in VS Code to understand their structure.
- Identified suspicious authentication-related activity, including:
  - Failed login attempts
  - Invalid or unknown users
  - Repeated suspicious access patterns

### 2. Python Log Analysis Automation
- Built a Python script to analyse a selected range of log entries.
- Searched for suspicious keywords such as:
  - `failed password`
  - `authentication failure`
  - `invalid user`
  - `user unknown`
- Stored matching entries in a suspicious events list.
- Categorised events by type.
- Counted the total number of suspicious events found.
- Exported the results to a CSV file for further review.

### 3. Splunk Enterprise SIEM Visualisation
- Ingested and indexed the Linux log file into Splunk Enterprise.
- Configured the log source and sourcetype.
- Used Splunk search queries to filter authentication-related events.
- Explored:
  - Event View
  - Pattern View
  - Statistics View
  - Visualisations for attack trend analysis

---

## Tools & Technologies

- Python
- VS Code
- Splunk Enterprise
- CSV Export
- Linux Log Dataset
- Basic SOC Analysis Workflow

---

## Repository Structure

```text
soc-log-analysis-python-splunk/
│
├── Log_analysis.py
├── README.md
│
├── data/
│   └── Linux_2k.log
│
└── results/
    └── suspicious_logs.csv
