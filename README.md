# Credit Card Fraud Detection – Power BI & ETL Pipeline

## Overview
Analyzed 999,000+ credit card transactions to identify 
fraudulent patterns and behaviour using Power BI Desktop 
and a fully structured ETL pipeline in Power Query.

## Problem Statement
Credit card fraud causes billions in losses annually. 
This project explores transaction-level data to uncover 
when, where, and how fraud occurs — and communicates 
findings through interactive dashboards.

## Tools & Technologies
- Power BI Desktop
- Power Query (M Language)
- ETL Pipeline (Extract, Transform, Load)
- Star Schema Data Modelling
- DAX (Data Analysis Expressions)

## ETL Process
- Extracted two raw datasets (transactions_train & transactions_test)
- Appended and merged 999,000+ rows using Power Query
- Engineered calculated columns:
  - Age Group (18-29, 30-44, 45-59, 60+)
  - Amount Band (<$10, $10-$49, $50-$199, $200+)
  - Fraud Label (Legitimate / Fraudulent)
  - Transaction Hour, Month, Year
  - Month Name (using M language date functions)
- Validated 100% column quality — 0% errors, 0% empty values
- Applied data type transformations at each pipeline step

## Data Model
Built a star schema with:
- Fact Table: transactions_Master
- Dim_Date — transaction year, month, hour, day of week
- Dim_Card — cardholder age, age group, date of birth
- Dim_Category — merchant category
- Dim_Merchant — merchant name, location coordinates
- Dim_State — city, state, population, coordinates

## Dashboards
3 storytelling dashboards built in Power BI:
1. Fraud Overview — overall fraud rate, trends by category and time
2. Behavioural Patterns — fraud by age group, transaction hour, amount band
3. Geographic Analysis — fraud distribution by state and city population

## Key Findings
- Fraud concentrated in specific merchant categories
- Higher fraud rates during late night transaction hours
- Certain age groups and amount bands show elevated fraud risk
- Geographic clusters of fraudulent activity identified

#Screenshots
<img width="1397" height="783" alt="11" src="https://github.com/user-attachments/assets/490af610-9d9b-4e1e-af0c-46dd400d17c5" />
<img width="1383" height="775" alt="22" src="https://github.com/user-attachments/assets/14fc08cc-0529-4838-a075-e03a3fc0d7c7" />
<img width="1405" height="785" alt="33" src="https://github.com/user-attachments/assets/476ae9a5-c3fe-420a-a31a-54a3ab7b3b8e" />


## Dataset
Source: Course-assigned dataset — Lambton College, 
Business Intelligence Tools (2026)
