# 🏥 Hospital General Information Dashboard

## Project Overview

This repository contains the source files and documentation for the **Hospital General Information Dashboard**, an interactive Power BI report designed to assess and analyze the performance of hospitals across the United States.

**Objective:** To enable healthcare administrators and policymakers to compare hospitals by geography, ownership, and type, identify quality gaps (e.g., mortality, readmissions), and explore 'What-If' policy scenarios.

## 🚀 Key Features

* **Systemic Gap Analysis:** Instantly identifies the most vulnerable performance domains (e.g., Mortality) using clustered visual comparisons.
* **Targeted Identification:** Pinpoints specific hospital types (e.g., Acute Care) driving poor quality scores.
* **"What-If" Scenario Modeling:** Includes dynamic sliders to simulate the impact of policy changes (e.g., setting a new **Rating Threshold** or modeling **Measure Improvement**).
* **Diagnostic Drill-Through:** Allows users to right-click a facility and view its complete, detailed scorecard.

## ⚙️ Technical Stack

| Component | Tool/Language | Purpose |
| :--- | :--- | :--- |
| **Data Source** | `Hospital_General_Information.csv` | Raw hospital performance data (38 columns). |
| **Visualization** | Power BI Desktop (`.pbix`) | Report development, visualization, and deployment source. |
| **Data Transformation** | Power Query (M Language) | Cleaning anomalies (e.g., handling "Not Available" strings) and feature engineering. |
| **Logic/Metrics** | Data Analysis Expressions (DAX) | Creating core metrics (e.g., `% High-Performing`) and complex scenario logic. |
| **Data Model** | Star Schema | Optimized structure for performance, linking a central Fact table (Hospitals) to Dimension tables (State, Ownership, Type). 


## 👥 Team Contribution

This project was developed by:

| Member | Primary Role | Key Deliverables |
| :--- | :--- | :--- |
| **Deeksha** | Data Ingestion & Cleaning | Power Query steps, Overview Page (Page 1). |
| **Vaishnavi** | Data Modeling & Documentation | Star Schema setup, Performance Details Page (Page 3). |
| **Deepak** | Core DAX Metrics & Visuals | Aggregated metrics, Geographic Analysis Page (Page 2). |
| **Sukesh** | Scenario Logic & Insights | "What-If" DAX sliders, Scenario Insights Page (Page 4). |

## 💻 Setup and Access

### Prerequisites

1.  **Power BI Desktop:** Required to open and modify the `.pbix` file.
2.  **Dataset:** The `Hospital_General_Information.csv` file must be saved locally and linked correctly as the data source in the Power BI file.

### Steps to Run Locally

1.  Clone this repository to your local machine.
    ```bash
    git clone [Your Repository URL]
    ```
2.  Ensure the `Hospital_General_Information.csv` file is in the same folder as the `.pbix` file, or update the source path in Power Query.
3.  Open the `Capstone Project _ Hospital Gen Info_Batch5.pbix` file using Power BI Desktop.
4.  If prompted, click **Apply Changes** to refresh the model with the local data.

### Deployment

The latest version of the dashboard is deployed and available for stakeholder review in the designated Power BI Service Workspace.

* **Workspace:** [Insert Power BI Workspace Name Here]
* **Access:** Permissions are managed via the Workspace settings. Contact **[Vaishnavi's Name]** for access or refresh schedule changes.

## 📚 Documentation

The detailed project documentation, including the User Guide, Technical Summary, and Anomaly Log, is provided in the `Documentation/` folder.

* **User Guide:** Explains navigation, slicers, and "What-If" scenarios.
* **Technical Document:** Contains the ERD, M-Query steps, and all final DAX formulas.

---
