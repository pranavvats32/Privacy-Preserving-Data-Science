# Privacy-Preserving Data Science

## Overview
This project focuses on anonymizing sensitive event logs (e.g., healthcare data) while preserving essential process patterns. By applying privacy techniques such as differential privacy and k-anonymity, the goal is to protect confidential information while maintaining the utility of process mining insights.

## Features
- **Anonymization Methods:** Implements differential privacy and k-anonymity for event log sanitization.
- **Utility Measurement:** Evaluates the impact of anonymization on process patterns.
- **Process Mining Compatibility:** Ensures anonymized logs remain usable for process mining analysis.

## Datasets

[Adult Census Income](https://www.kaggle.com/datasets/uciml/adult-census-income?resource=download)

[Synthetic Data from a Financial Payment System](https://www.kaggle.com/datasets/ealaxi/banksim1)

[Medical Costs Personal Datasets](https://www.kaggle.com/datasets/mirichoi0218/insurance)

[BPI Challenge 2017](https://data.4tu.nl/articles/dataset/BPI_Challenge_2017/12696884)

## How to Apply k-Anonymity for These Datasets:

Identify Sensitive Attributes: Look for fields like customer ID, income, loan amount, account number, transaction amounts, etc., which need to be anonymized.
  
Choose an Anonymization Strategy: Use techniques like:

- Generalization: Replace precise values with broader categories (e.g., age group instead of exact age).

- Suppression: Remove highly specific values that make an individual identifiable.

- Bucketization: Group similar records together to hide individual data points.

Measure the Impact: Ensure that the anonymization preserves the utility of the data for analysis (such as identifying trends or patterns in banking operations).

Use Tools for Process Mining: Convert the anonymized data into XES format using tools like ProM, Celonis, or Python scripts, and analyze the process logs for insights.


## Deliverables
- **Code** for event log anonymization.
- **Utility measurement** to assess data
- a retention quality.


