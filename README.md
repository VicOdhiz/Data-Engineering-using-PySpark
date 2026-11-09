# IEBC 2022 Voter Registration Analytics – PySpark & Power BI

## 1. Project Overview

This project implements an end-to-end data engineering and analytics solution using Kenya's 2022 Independent Electoral and Boundaries Commission (IEBC) voter registration statistics.

The project demonstrates how raw electoral data published in PDF documents can be transformed into structured, analytics-ready datasets using Apache PySpark, stored in Delta Lake, and presented through interactive Power BI dashboards.

The solution provides insights into voter registration distribution across counties, constituencies, wards and polling stations.

It also demonstrates practical implementation of data engineering concepts, including data extraction, transformation, data quality validation, data modelling and business intelligence.

## 2. Project Objectives

- Extract voter registration statistics from raw IEBC PDF documents.
- Transform unstructured data into structured datasets using PySpark.
- Clean and standardise geographical identifiers and voter registration figures.
- Implement a data processing pipeline using Apache Spark.
- Store transformed datasets in Delta Lake.
- Develop relational data models to support analytical queries.
- Build interactive Power BI dashboards.
- Implement Row-Level Security (RLS) for controlled access to geographical data.

## 3. Technology Stack

| Technology | Purpose |
|---|---|
| Python | Data processing and scripting |
| Apache PySpark | Distributed data processing and transformation |
| Databricks | Spark development and execution environment |
| Delta Lake | Structured data storage |
| Power BI | Data visualisation and reporting |
| DAX | Analytical calculations and measures |
| SQL | Data querying and validation |

## 4. Data Engineering Architecture

The project follows a structured data processing approach.

**Pipeline:**

1. **Source Layer:** Raw IEBC 2022 voter registration PDF documents.
2. **Extraction:** Extract voter registration statistics from PDF documents.
3. **Transformation:** Use PySpark to clean, standardise and validate the extracted datasets.
4. **Storage:** Load processed datasets into Delta Lake tables.
5. **Data Modelling:** Establish relationships between geographical dimensions and voter registration facts.
6. **Analytics:** Connect Power BI to the transformed datasets to develop interactive dashboards.

## 5. Data Transformation and Processing

Apache PySpark was used to perform the following operations:

- Data extraction and loading.
- Handling missing and inconsistent values.
- Data type standardisation.
- Standardisation of county, constituency and ward codes.
- Cleaning numerical voter registration figures.
- Validation of geographical identifiers.
- Handling duplicate and inconsistent records.
- Preparation of analytics-ready datasets.

Particular attention was given to maintaining consistent geographical codes to ensure referential integrity across the datasets.

## 6. Data Model

The solution uses a relational data model connecting geographical dimensions to voter registration statistics.

**Core datasets include:**

- Counties
- Constituencies
- Wards
- Polling Stations
- Voter Registration Statistics

The relationships enable geographical drill-down analysis from county level to individual polling stations.

## 7. Power BI Analytics

The transformed Delta Lake datasets were connected to Power BI to develop interactive dashboards.

The analytical solution supports:

- Voter registration distribution by county.
- Constituency-level voter registration analysis.
- Ward-level comparisons.
- Polling station-level analysis.
- Geographical drill-down and filtering.
- Comparative analysis of voter registration statistics.

DAX measures were used to support analytical calculations and dashboard reporting.

### Row-Level Security (RLS)

Row-Level Security was implemented to demonstrate controlled access to geographical data, ensuring users can access information according to their assigned security roles.

## 8. Key Data Engineering Concepts Demonstrated

This project demonstrates practical experience in:

- ETL pipeline development.
- Apache Spark and PySpark transformations.
- Delta Lake storage.
- Data cleansing and standardisation.
- Data quality checks and validation.
- Relational data modelling.
- Fact and dimension table design.
- Data integration.
- BI reporting and dashboard development.
- Role-Based Data Access through Power BI RLS.

## 9. Business Value

The project transforms static electoral statistics into structured, accessible and interactive analytical information.

It demonstrates how data engineering technologies can be applied to public-sector datasets to improve data accessibility, geographical analysis, reporting and evidence-based decision-making.

## 10. Project Outcome

An end-to-end analytics solution demonstrating the integration of Python, Apache PySpark, Databricks, Delta Lake and Power BI to transform raw PDF-based voter registration statistics into structured datasets and interactive dashboards.

---

**Author:** Victor Odhiambo

**Project Category:** Data Engineering | Data Analytics | Business Intelligence

**Technologies:** Python | PySpark | Databricks | Delta Lake | Power BI | DAX
