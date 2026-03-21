# Canadian Federal Workforce Analytics Dashboard

*A public-sector HR reporting case study built in Power BI using official Canadian federal public service workforce data.*

## Project at a Glance

- **Domain:** HR / Workforce Analytics  
- **Tool:** Power BI  
- **Data sources:** Official Canadian federal public service workforce datasets  
- **Time period:** 2010–2025  
- **Focus areas:** Workforce trends, department comparison, tenure structure, age profile, geographic distribution  
- **Project type:** Portfolio case study for junior HR Data Analyst / HR Reporting Analyst roles

##Dashboard Preview
<img width="1051" height="602" alt="image" src="https://github.com/user-attachments/assets/8718acf6-b9da-4128-a6f2-950ad7e93393" />
<img width="951" height="533" alt="image" src="https://github.com/user-attachments/assets/e2e24170-a359-48d5-b9d2-7e42a5562501" />
<img width="1046" height="607" alt="image" src="https://github.com/user-attachments/assets/f839259e-d71e-4628-80d2-a5238b79554a" />

## Project Overview

This project analyzes publicly available Canadian federal public service workforce data to support HR reporting and workforce planning. It focuses on workforce size, department distribution, tenure structure, age profile, and geographic distribution across the federal public service.

The project was designed to demonstrate practical HR reporting and workforce analytics skills using real public data. It reflects the type of work involved in turning raw workforce files into usable reporting outputs: cleaning and structuring data, defining KPIs, building dashboard views, documenting assumptions, and presenting business-relevant findings.

## Business Problem

HR and business leaders need reliable workforce reporting to understand how the public service has changed over time, where workforce concentrations exist, and what structural patterns may affect planning and decision-making.

Public workforce data exists across multiple files, but it must be cleaned, standardized, and documented before it can support consistent reporting and comparison.

## Project Objectives

- Consolidate multiple public workforce datasets into a clean reporting model  
- Analyze workforce trends from 2010 to 2025  
- Compare departments and agencies across workforce size and composition measures  
- Build an interactive Power BI dashboard for HR reporting  
- Document KPI definitions, assumptions, and data limitations  

## Scope of Version 1

### Included
- Total workforce trend  
- Department trend analysis  
- Tenure analysis  
- Age-band analysis  
- Province/territory workforce distribution  
- Department comparison over a selected period  

### Excluded
- Hires  
- Terminations  
- Turnover  
- Employee-level HRIS logic  
- Predictive modeling  
- Advanced statistical modeling  
- Employee experience survey analysis (deferred after initial profiling due to complexity)  

## Data Sources

This project uses official public datasets from the Government of Canada, including:

- Population of the federal public service  
- Population of the federal public service by department or agency  
- Population of the federal public service by department and tenure  
- Population of the federal public service by department and age band  
- Population of the federal public service by department and province or territory of work  

## Data Preparation

The source files were cleaned and standardized before modeling in Power BI. Key preparation steps included:

- Renaming fields into a consistent naming convention  
- Standardizing employee count fields across tables  
- Keeping source datasets as separate reporting tables rather than forcing them into one merged table  
- Removing pre-aggregated total rows from granular analysis tables  
- Creating shared dimensions for year and department  
- Creating a custom age-band sort structure for reporting visuals  
- Creating a simplified map field for province/territory reporting  
- Handling suppressed values and documenting related limitations  

## Data Model

The dashboard was built using separate fact-like tables connected through shared dimensions.

### Core tables
- `population_overall`
- `department_population`
- `department_tenure_type`
- `department_age_band`
- `department_work_location`

### Dimension tables
- `dim_year`
- `dim_department`

This structure supports consistent filtering across dashboard pages while keeping each source aligned to its original reporting grain.

## Dashboard Pages

## 1. Executive Overview

Provides a high-level summary of workforce size and structure, including:

- Total employees  
- Number of departments/agencies  
- Top departments by headcount  
- Workforce composition by organization type  
- Long-term workforce trend  

## 2. Workforce Composition

Shows workforce structure across:

- Tenure type  
- Age band  
- Geographic distribution  
- National Capital Region workforce count  
- Outside Canada workforce count  

## 3. Department Analysis

Provides deeper department-level comparison, including:

- Headcount change over the selected period  
- Department comparison summary  
- Top department headcount trends over time  

## Key KPIs

- Total federal public service population  
- Number of reporting departments/agencies  
- Employees in latest selected year  
- Employees in earliest selected year  
- Headcount change over selected period  
- Headcount change percentage over selected period  
- Workforce composition by organization type  
- Workforce composition by tenure type  
- Largest age band  
- National Capital Region employees  
- Outside Canada employees  

## Sample Findings

- Federal workforce size increased materially over the later part of the reporting period.  
- Workforce composition is heavily concentrated in indeterminate employees.  
- Mid-career age bands represent the largest share of the workforce.  
- Workforce distribution is concentrated in specific provinces/territories and in the National Capital Region.  
- Department growth is uneven, with some organizations expanding much more than others over the selected period.  

## Assumptions and Limitations

- The datasets are aggregate, not employee-level.  
- This project supports workforce reporting, not operational HRIS analytics.  
- Hires, terminations, and turnover cannot be calculated directly from the selected public aggregate datasets.  
- Some source files contain suppressed values, which were handled for reporting purposes and documented as a limitation.  
- Geography data includes special categories such as National Capital Region and Outside of Canada, which required separate handling for mapping.  
- This version focuses on descriptive reporting rather than causal or predictive analysis.  

## Technical Highlights

- Cleaned and standardized multiple public workforce datasets  
- Built a multi-table reporting model in Power BI  
- Created shared dimensions for year and department filtering  
- Used DAX measures for headcount, selected-period change, and summary KPIs  
- Designed a 3-page dashboard for HR reporting and workforce planning use  

## Tools Used

- Excel  
- Power Query / data cleaning logic  
- Power BI  
- DAX  
- GitHub documentation  

## Repository Contents

- `canadian_federal_workforce_analytics_dashboard.pbix` — Power BI dashboard file  
- `README.md` — Project overview and methodology  
- `kpi_definitions.md` — KPI descriptions and business logic  
- `assumptions_and_limitations.md` — Key data assumptions and reporting limitations  
- `findings_and_recommendations.md` — Summary findings and portfolio-style recommendations  

## Why This Project Matters

This project was designed to reflect practical HR reporting work: collecting public data, cleaning and structuring it, defining business KPIs, building reporting views, and translating workforce data into usable insight.

It also demonstrates an important constraint often found in real analytics work: producing useful reporting from imperfect, aggregate, and non-HRIS data while being transparent about what the data can and cannot support.
