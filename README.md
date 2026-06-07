# Adey Innovations - Fraud Detection System

## Overview

This project aims to detect fraudulent transactions across two distinct streams:

1. E-commerce: Featuring contextual user data and IP-based geolocation.
2. Credit Card: Featuring anonymized PCA-transformed features.

## Project Structure

- `notebooks/`: Contains the step-by-step EDA and feature engineering.
- `data/`: Contains raw and processed files (excluded from git).

## Key Deliverables (Task 1)

- **Data Cleaning**: Handled missing values and date conversions.
- **Geolocation Enrichment**: Mapped IP addresses to countries using `pd.merge_asof` to identify high-risk origin points.
- **Feature Engineering**: Engineered behavioral features (`time_since_signup`, `device_count`) to capture fraud patterns.
- **Handling Imbalance**: Identified severe class imbalance and prepared the workflow for SMOTE (to be applied in the modeling phase).
