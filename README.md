# 💳 Payment Card Fraud Analytics

## 📌 Project Overview

This project was developed as part of the Ironhack Data Analytics Bootcamp.

The objective was to analyze payment card fraud using relational databases and SQL to identify the transaction patterns, account characteristics, and network behaviors most strongly associated with fraudulent activity.

The project combines Python based data preparation with MySQL database design and SQL analysis to transform multiple fraud datasets into actionable business insights.

## 🎯 Business Problem

Payment card fraud creates significant financial losses and operational risk for financial institutions.

Fraud detection requires understanding not only individual fraudulent transactions, but also the account characteristics, transaction behaviors, and network relationships associated with higher fraud risk.

This project uses structured fraud data to identify high risk patterns and support more targeted fraud monitoring and investigation.

## 💡 Business Hypothesis

Fraud risk is concentrated around identifiable transaction characteristics, higher risk account profiles, and connected account networks.

By analyzing these factors together, financial institutions can better identify the patterns associated with financial losses and coordinated fraud activity.

## ❓ Research Questions

The analysis focuses on four business questions:

1. Which fraud patterns generate the highest financial losses?

2. Which account characteristics are associated with higher fraud risk?

3. Which transaction characteristics are most commonly associated with fraudulent activity?

4. Can network analysis identify coordinated fraud rings and high risk account clusters?

## 📊 Data Sources

The project uses five fraud analytics datasets.

### Transactions

Transaction level data including transaction amount, merchant category, device type, foreign transaction indicators, IP risk score, transaction velocity, and fraud status.

### Account Profiles

Account level characteristics including account type, account age, risk score, two factor authentication status, and fraud history.

### Fraud Patterns

Aggregated fraud pattern information used to evaluate fraud frequency and financial impact.

### Network Edges

Relationships between connected accounts and identified fraud rings, supporting the analysis of coordinated fraud activity.

### Time Series Statistics

Fraud metrics across time periods used to analyze fraud activity and trends.

The full transaction datasets are excluded from this repository because they exceed GitHub's 100 MB file size limit.

## 🔧 Methodology

The project followed these main steps:

1. Dataset inspection and validation
2. Data cleaning and preparation in Python
3. Primary key validation
4. Foreign key and dataset relationship validation
5. Data type and column standardization
6. Clean dataset export for MySQL
7. Relational database creation
8. SQL based exploratory analysis
9. Business question analysis
10. Fraud insight and recommendation development

## 🗄 Database Structure

The cleaned datasets were structured into five relational database tables:

`transactions`

`account_profiles`

`fraud_patterns`

`network_edges`

`time_series_stats`

Primary and foreign key relationships were reviewed to support data integrity and cross table analysis.

## 🔍 SQL Analysis

The SQL analysis was structured around four research areas.

### Financial Impact of Fraud Patterns

Identifies fraud patterns associated with the highest total financial losses and evaluates fraud frequency and severity.

### Account Fraud Risk

Analyzes account characteristics including risk score, account age, account type, and two factor authentication status.

### Transaction Fraud Characteristics

Evaluates transaction characteristics including merchant category, device type, foreign transactions, IP risk score, and transaction velocity.

### Network Fraud Analysis

Analyzes shared account connections and fraud ring structures to identify highly connected clusters and coordinated fraud activity.

## 📂 Repository Structure

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

## 🛠 Technologies Used

Python

Pandas

Jupyter Notebook

MySQL

MySQL Workbench

SQL

Visual Studio Code

Git

GitHub

## 👥 Team

Team Winifred & Sevgi

Winifred

Sevgi Özdemir

Ironhack Data Analytics Bootcamp

## 📋 Project Management

The project was managed using an Agile workflow in Trello, including sprint planning, task assignment, progress tracking, and collaboration throughout the project.

Trello Board:

https://trello.com/b/Bx7wiGFC/winifred-sevgi

## 📽 Presentation

Presentation Slides:

https://docs.google.com/presentation/d/1zezE-2GEEpBFHoSCLyrewtu6iUBaoYea3pJn2T3Ktz0/edit?slide=id.p1#slide=id.p1

## 📜 License

This project was created for educational purposes as part of the Ironhack Data Analytics Bootcamp.