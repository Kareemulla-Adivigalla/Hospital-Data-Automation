# Hospital Data Automation

## Project Overview

This project automates the daily loading of hospital billing data from Excel files into SQL Server.

The solution eliminates manual import activities and prepares the data for Power BI reporting.

---

## Business Problem

Every day, billing data was exported from the hospital system into Excel.

The manual process included:

- Exporting Excel files
- Cleaning columns
- Renaming fields
- Mapping data
- Importing into SQL Server

The process consumed approximately 5 hours per day.

---

## Solution

A PowerShell-based automation process was developed to:

1. Read Excel files automatically
2. Load data into SQL Server staging tables
3. Perform validation checks
4. Update reporting tables
5. Send processed data to Power BI

---

## Technologies Used

- SQL Server
- PowerShell
- Excel
- Windows Task Scheduler
- Power BI

---

## Workflow

Excel Files
↓
Staging Tables
↓
Validation
↓
Fact Tables
↓
Power BI Dashboard

---

## Key Features

### Full Load

Loads complete Excel extract into staging area.

### Incremental Load

Adds only new transactions into reporting tables.

### Automation

Supports scheduled execution through Windows Task Scheduler.

### Data Validation

Ensures data quality before loading.

---

## Project Impact

| Metric | Before | After |
|----------|----------|----------|
| Daily Processing Time | 5 Hours | 30 Minutes |
| Manual Steps | 10+ | 2 |
| Human Errors | High | Very Low |

---

## Future Enhancements

- Email Monitoring
- Automated Alerts
- SSIS Package Integration
- Microsoft Fabric Integration
