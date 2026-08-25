# Machine Learning-Based Prediction of Merchant Transaction Volume and Onboarding Patterns Across Multi-Country Payment Networks: A Case Study of Arab Financial Services (AFS)

MSc Artificial Intelligence — Bahrain Polytechnic
Author: Maram Alkhenaizi
Supervisor: Mr. Husain Naser

## Overview

This repository contains the code for an MSc thesis on revenue forecasting and merchant
analytics for a multi-country payment processor (AFS), covering markets in Bahrain, Oman,
Egypt, and the UAE.

The project has two objectives:

1. **Revenue forecasting** — predicting daily settlement profit using time-series and machine
   learning models.
2. **Merchant value classification** — classifying newly onboarded merchants by potential value
   tier (Low/Medium/High) using early-life transaction behavior.

## Data Availability

**The datasets are not included in this repository.** All data consists of **real, confidential
transaction records provided by AFS** and cannot be shared publicly due to data-privacy and
institutional confidentiality restrictions.

The code is provided for methodology review. To reproduce the analysis, you will need your own
dataset matching the expected structure below.

## Reproducibility

To run the notebooks with your own data:

1. Clone this repository.
2. Install dependencies from `Requirements.txt`.
3. Place your dataset(s) in a local `data/` folder.
4. Update the file path variable at the top of each notebook to point to your dataset.
5. Ensure your dataset columns match the expected schema below — the notebooks reference these
   column names directly.

### Objective 1 — Revenue Forecasting

Each notebook expects a daily revenue dataset with the columns:

`Settlement Date`, `Transaction Count`, `Transaction Amount`, `Average Transaction Amount`, `Profit`

### Objective 2 — Merchant Value Classification

Each notebook expects a monthly per-merchant dataset with the columns:

`MID`, `Transactions Count`, `Transaction Amount`, `Average Transaction Amount`, `DATASOURCE`, `Settlement Month`, `Settlement Year`, `isActive`, `status`, `riskLevel`, `BusinessType`, `OnboardingDate`

## Repository Structure

```
code/
├── objective1_revenue_forecasting/   # Notebooks for daily revenue forecasting per region
└── objective2_merchant_classification/  # Notebooks for merchant value classification per region
```
