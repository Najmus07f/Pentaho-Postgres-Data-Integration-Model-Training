# End-to-End-Data-Pipeline-ML-Modeling-with-Pentaho-PostgreSQL-DWH
Overview

This repository contains an end-to-end workflow: ETL in Pentaho, a star-schema warehouse in PostgreSQL (dimensions + fact), and ML notebooks in Python. The goal is to move from raw data to reliable features, predictions, and structure discovery.

Data Flow

Source → Pentaho ETL → PostgreSQL DWH → Python Notebooks (ML & reports).
The warehouse uses a central fact table and clear dimension tables (e.g., Date, Entity/Category/Geography) with keys, constraints, and helpful indexes.

Preprocessing

Missing-value handling, type casting, categorical encoding, scaling/normalization, and basic outlier review. Multiple variants are tested to see what helps model performance.

Models

Supervised (Regression): Ridge Regression, Decision Tree Regressor, Random Forest Regressor

Unsupervised: K-Means clustering (group discovery), Isolation Forest (anomaly detection)

Evaluation (placeholders)

Report MAE/RMSE/R² for regressors; silhouette/cluster summaries for K-Means; anomaly rates and examples for Isolation Forest.
Dataset:https://www.kaggle.com/datasets/cityofLA/los-angeles-parking-citations?select=parking-citations.csv
