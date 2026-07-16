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
   learning models (completed).
2. **Merchant potential classification** — classifying merchants by value tier and predicting
   new-merchant potential from early activity (not yet started).

## Data Availability

**The datasets are not included in this repository.** All data consists of **real, confidential
transaction records provided by AFS** and cannot be shared publicly due to data-privacy and
institutional confidentiality restrictions.

The code is provided for methodology review. Each notebook expects a daily revenue dataset with
the columns: `Settlement Date`, `Transaction Count`, `Transaction Amount`,
`Average Transaction Amount`, and `Profit`.
