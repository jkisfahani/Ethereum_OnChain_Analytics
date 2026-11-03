# Ethereum On-Chain Analytics

## Project Overview

This project analyzes Ethereum blockchain transaction data using Python, SQL, DuckDB, and AWS Public Blockchain Data stored in Amazon S3.

The goal is to extract meaningful insights from on-chain transaction activity, examine network usage patterns, and build practical blockchain data analytics skills.

## Objectives

- Analyze Ethereum transaction activity.
- Measure successful and failed transactions.
- Explore hourly transaction patterns.
- Compare transaction types and failure rates.
- Analyze gas consumption and estimated transaction fees.
- Query large Parquet datasets directly from Amazon S3 using DuckDB.

## Technology Stack

- **Python** — Data analysis and processing
- **Pandas** — Data manipulation
- **DuckDB** — SQL analytics on Parquet data
- **Matplotlib** — Data visualization
- **Jupyter Notebook** — Interactive analysis
- **AWS S3** — Public blockchain data source
- **Git & GitHub** — Version control and project documentation

## Data Source

- **Provider:** AWS Public Blockchain Data
- **Blockchain:** Ethereum
- **Format:** Apache Parquet (`.snappy.parquet`)
- **Storage:** Amazon S3
- **Access:** Public dataset; no AWS credentials required for the files analyzed here.

## Project Structure

```text
Ethereum_OnChain_Analytics/
│
├── notebooks/
│   └── 01_Ethereum_Data_Exploration.ipynb
│
├── 01_Python_Environment_Test.ipynb
├── 02_Ethereum_AWS_S3_Analytics.ipynb
│
├── ethereum_gas_analysis.csv
├── ethereum_hourly_analysis.csv
├── ethereum_transaction_types.csv
│
├── .gitignore
└── README.md
```

## Key Findings

Initial analysis of Ethereum transactions for October 28, 2026:

| Metric | Result |
|---|---:|
| Total transactions | 1,996,106 |
| Successful transactions | 1,971,694 |
| Failed transactions | 24,412 |
| Success rate | 98.78% |
| Failure rate | 1.22% |
| Estimated total transaction fees | 110.4208 ETH |

### Transaction Type Analysis

- EIP-1559 (Type 2) represented approximately 76.58% of transactions.
- Legacy transactions (Type 0) represented approximately 21.29%.
- EIP-7702 (Type 4) had a failure rate of approximately 2.44% in this sample.

*These findings describe a one-day sample and should not be interpreted as long-term network trends.*

## Visualizations

The notebooks include visual analysis of:

- Hourly transaction activity.
- Successful versus failed transactions.
- Hourly transaction failure rates.
- Failure rates by transaction type.
- Average gas consumption for successful and failed transactions.

## Current Status

**Phase 1 — Initial Data Exploration and Analytics**

Completed:
- Python environment testing.
- Public Ethereum S3 data access.
- DuckDB SQL analysis.
- Transaction and gas analysis.
- CSV exports.
- Initial GitHub publication.

Future work:
- Expand the analysis across multiple dates.
- Build historical Ethereum activity datasets.
- Develop deeper on-chain analytics.
- Create a professional analytics dashboard.

## Author

GitHub: [@jkisfahani](https://github.com/jkisfahani)
