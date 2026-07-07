# Payment Card Fraud Analytics

## Project Overview

Payment card fraud creates significant financial losses and operational risk for financial institutions.

This project analyzes transaction, account, fraud pattern, time series, and network data to identify the characteristics and behavioral patterns most strongly associated with fraudulent activity.

The analysis combines Python for data preparation and MySQL for database design and business analysis.

## Business Case

A financial institution wants to improve its understanding of payment card fraud by identifying the transaction patterns, account characteristics, and network behaviors associated with fraudulent activity.

The objective of this project is to use structured data analysis to identify high risk fraud patterns and translate the findings into actionable business insights.

## Business Questions

The project focuses on four research questions:

1. Which fraud patterns generate the highest financial losses?

2. Which account characteristics are associated with higher fraud risk?

3. Which transaction characteristics are most commonly associated with fraudulent activity?

4. Can network analysis identify coordinated fraud rings and high risk account clusters?

## Data Sources

The project uses five datasets:

### Transactions

Contains transaction level information including transaction amount, merchant category, device type, foreign transaction indicators, IP risk score, transaction velocity, and fraud status.

### Account Profiles

Contains account level characteristics including account type, account age, risk score, two factor authentication status, and fraud history.

### Fraud Patterns

Contains aggregated fraud pattern information used to evaluate fraud frequency and financial impact.

### Network Edges

Contains relationships between connected accounts and identified fraud rings, supporting the analysis of coordinated fraud activity.

### Time Series Statistics

Contains fraud metrics across time periods to support trend and temporal analysis.

The full transaction datasets are excluded from this repository because they exceed GitHub's 100 MB file size limit.

## Data Preparation

Data preparation was completed in Python using Jupyter Notebook.

The main preparation steps included:

1. Loading and inspecting all source datasets

2. Reviewing column names, data types, and missing values

3. Validating primary key uniqueness

4. Validating relationships between datasets

5. Standardizing data types and column structures

6. Preparing cleaned datasets for MySQL import

7. Exporting cleaned CSV files for database creation

The data preparation workflow is available in:

`notebooks/01_Data_preparation.ipynb`

## Database Structure

The cleaned datasets were imported into MySQL and structured as relational tables.

The main database tables are:

`transactions`

`account_profiles`

`fraud_patterns`

`network_edges`

`time_series_stats`

Primary and foreign key relationships were reviewed to support data integrity and SQL analysis.

## SQL Analysis

The SQL analysis includes database creation, table preparation, data validation, and queries designed to answer the four business research questions.

The complete SQL analysis is available in:

`sql/SQL_Merged_Database&Analysis.sql`

## Tools and Technologies

Python

Pandas

Jupyter Notebook

MySQL

MySQL Workbench

SQL

Visual Studio Code

Git

GitHub

## Repository Structure

```text
SQL_Mini_Project/
│
├── cleaned_data/
│   ├── account_profiles_clean.csv
│   ├── fraud_patterns_clean.csv
│   ├── network_edges_clean.csv
│   └── time_series_stats_clean.csv
│
├── data/
│   ├── account_profiles.csv
│   ├── fraud_patterns.csv
│   ├── network_edges.csv
│   └── time_series_stats.csv
│
├── notebooks/
│   └── 01_Data_preparation.ipynb
│
├── sql/
│   └── SQL_Merged_Database&Analysis.sql
│
├── .gitignore
│
└── README.md

## Presentation

The final project presentation is available here:

[View the Payment Card Fraud Analytics Presentation]: https://docs.google.com/presentation/d/1zezE-2GEEpBFHoSCLyrewtu6iUBaoYea3pJn2T3Ktz0/edit?slide=id.p1#slide=id.p1