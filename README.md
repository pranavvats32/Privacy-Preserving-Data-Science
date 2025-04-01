# Privacy-Preserving Process Mining

## Overview
This project focuses on anonymizing sensitive event logs (e.g., healthcare data) while preserving essential process patterns. By applying privacy techniques such as differential privacy and k-anonymity, the goal is to protect confidential information while maintaining the utility of process mining insights.

## Features
- **Anonymization Methods:** Implements differential privacy and k-anonymity for event log sanitization.
- **Utility Measurement:** Evaluates the impact of anonymization on process patterns.
- **Process Mining Compatibility:** Ensures anonymized logs remain usable for process mining analysis.

## Datasets
[BPI Challenge 2017](https://data.4tu.nl/articles/dataset/BPI_Challenge_2017/12696884)
(Hospital Billing)
Description: Logs related to hospital billing, including invoices, payments, and financial transactions.

It involves patient financial data that must be anonymized while retaining process patterns.

[MIMIC 3 Dataset](https://physionet.org/content/mimiciii/1.4/)
Description: A massive dataset with ICU patient records, including lab results, medications, and diagnoses.

It provides rich event logs but requires de-identification due to its detailed patient data.
(Yet to acquire MIMIC in BigQuery)

[Uber & Lyft Ride-Sharing Data (New York City Jan 2024)](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
Description: Taxi and ride-sharing trip data, including timestamps, pickup/drop-off locations, and fares.

Contains personally identifiable information (PII) like GPS coordinates and timestamps, which need obfuscation.
(Dataset is available in PARQUET form, need to preprocess to XES)

[German Credit Dataset](https://archive.ics.uci.edu/dataset/144/statlog+german+credit+data)
Description: A dataset used for credit scoring, which contains attributes like credit history, personal details, and credit risk information for individuals.

It involves sensitive financial information such as income, loan amount, and other attributes that can be anonymized using k-anonymity.

How to Apply k-Anonymity for These Datasets:
Identify Sensitive Attributes: Look for fields like customer ID, income, loan amount, account number, transaction amounts, etc., which need to be anonymized.

Choose an Anonymization Strategy: Use techniques like:

Generalization: Replace precise values with broader categories (e.g., age group instead of exact age).

Suppression: Remove highly specific values that make an individual identifiable.

Bucketization: Group similar records together to hide individual data points.

Measure the Impact: Ensure that the anonymization preserves the utility of the data for analysis (such as identifying trends or patterns in banking operations).

Use Tools for Process Mining: Convert the anonymized data into XES format using tools like ProM, Celonis, or Python scripts, and analyze the process logs for insights.


## Deliverables
- **Code** for event log anonymization.
- **Utility measurement** to assess data retention quality.


