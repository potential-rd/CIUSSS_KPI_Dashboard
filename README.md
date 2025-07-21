# CIUSSS_KPI_Dashboard
A **Power BI**–based, scalable, and readable KPI dashboard for CIUSSS du Centre-Ouest-de-l'Île-de-Montréal staff to monitor hospital performance in real time.

---

## Table of Contents

1. [Description](#description)
2. [Tech Assets and URLs](#tech-assets-and-urls)
3. [Installation](#installation)
4. [Prerequisites](#prerequisites)
5. [Usage](#usage)
6. [Example](#example)
7. [Features](#features)
8. [Data Sources](#data-sources)
9. [Troubleshooting](#troubleshooting)
10. [Costs Involved](#costs-involved)
11. [Passwords and Credentials](#passwords-and-credentials)
12. [Contributing](#contributing)
13. [License](#license)
14. [Contact Information](#contact-information)

---

## Description

The **CIUSSS KPI Dashboard** is a community‑driven project that delivers a scalable, easy‑to‑read Power BI report for CIUSSS staff. It enables frontline and administrative users to:

* Track clinical and operational KPIs at a glance
* Compare performance over time and against targets
* Export visuals and data for external reporting

---

## Tech Assets and URLs

* **GitHub Repo:** [https://github.com/potential-rd/CIUSSS_KPI_Dashboard](https://github.com/potential-rd/CIUSSS_KPI_Dashboard)
* **Data File:** `HipKnee_Validated_KPIs.xlsx`
* **Dashboard File:** `CIUSSS_KPI_dashboard.pbix`
* **Power BI Service Workspace:** `CIUSSS KPI Dashboard` (requires CIUSSS account)

---

## Installation

1. **Clone the repository**

   ```bash
   git clone git@github.com:potential-rd/CIUSSS_KPI_Dashboard.git
   cd ciusss-kpi-dashboard
   ```
2. **Install Power BI Desktop** (Feb 2025 or later).
3. **Open the report**

   * Launch Power BI Desktop
   * File → Open → `dashboard/CIUSSS_KPI_Dashboard.pbix`
4. **Configure data source**

   * Home → Transform data → Data source settings
   * Point to `data/hospital_kpis.csv` or your Azure SQL instance

---

## Prerequisites

* **Power BI Desktop** (February 2025 version or later)
* **Access** to the source data (`.csv` or Azure SQL)
* 
---

## Usage

1. **Refresh data**

   * Home → Refresh
2. **Filter & drill‑down**

   * Use slicers at the top to select date ranges, facilities, or KPI categories
3. **Export**

   * Right‑click any visual → Export data (CSV) or Export to PowerPoint
4. **Publish**

   * File → Publish → Select your Power BI Service workspace

---

## Example

1. Open the “Main page” page to see high‑level metrics.
2. Select "Category" filter to see different KPI indicators.
3. Change "Year" to see hospital's performance on specific year.

---

## Features

* **Scalable model**: supports multiple date format and new KPIs
* **Responsive layout**: optimized for desktop, tablet, and email.
* **Custom filters**: date ranges, category, indicator
* **Automated refresh**: schedule via Data source
* **Export options**: CSV, PPTX, PDF
* **Accessibility**: high‑contrast themes and legible fonts

---

## Data Sources

* **HipKnee_Validated_KPIs.xlsx**

  * Columns: `Indicator family english	Indicator family french	Indicator english	Indicator french	Indicator desc english	Indicator desc french	2019-2020	2020-2021	2021-2022	Impact since last measurement`
  * Updated when new KPI available


---

## Troubleshooting

* **Visual rendering issues**

  * Ensure you’re on the latest Power BI Desktop build.
  * Clear the model cache: File → Options → Data Load → Clear cache.

---

## Costs Involved

* **Power BI Pro licenses** (billed monthly to CIUSSS IT budget)
* **Azure SQL** (if used): (billed monthly to CIUSSS IT budget)

---

## Passwords and Credentials

> **Never** commit secrets to this repo.

* **CSV Source**: no password
* **Azure SQL**: managed via Azure Key Vault; set `AZURE_SQL_USER` and `AZURE_SQL_PASSWORD` as env vars
* **Power BI Service**: login with CIUSSS SSO

---

## Contributing

1. **Fork** the repo
2. **Create a branch:** `git checkout -b feature/your-feature`
3. **Commit** your changes: `git commit -m "Add …"`
4. **Push** to your fork: `git push origin feature/your-feature`
5. **Open a PR** against `main`

---

## Contact Information
For any questions or concerns, please contact:
* **Project Lead:** Yifei Liu
* **Email:** [yifei.liu2@mail.mcgill.ca](mailto:yifei.liu2@mail.mcgill.ca)
* **GitHub:** [https://github.com/potential-rd/CIUSSS_KPI_Dashboard](https://github.com/potential-rd/CIUSSS_KPI_Dashboard)

