# BPS-MedPrice-Forecasting

# TreeMedPriceForecast

Machine Learning framework for spatio-temporal forecasting of public healthcare expenditure using tree-based models.

This repository contains the computational pipeline developed for the study:

**"Spatio-Temporal Forecasting of National Healthcare Expenditure: Benchmarking Tree Ensembles via Out-of-Time Validation"**

The objective of this work is to predict pharmaceutical acquisition expenditures for rheumatic and autoimmune diseases using public procurement data from the Brazilian Healthcare Price Database (Banco de Preços em Saúde - BPS).

The proposed framework evaluates five tree-based regression algorithms under a strict temporal validation strategy:

- Decision Tree
- Random Forest
- Extra Trees
- XGBoost
- LightGBM

---

## Repository Structure

```text
TreeMedPriceForecast/
├── TreeMedPriceForecast.ipynb
│   └── Main Colab/Jupyter pipeline
│       - Data preprocessing
│       - Feature engineering
│       - Model training
│       - Model evaluation
│       - Generation of tables and figures
│
├── data/
│   └── bps_rheumatic_autoimmune_procurement_1997_2025.parquet
│       └── Dataset used for model training and figure generation
│
├── results/
|   |
|   ├── csv/
|   |
│   ├── tables/
│   │
│   └── figures/
│     
│
├── README.md
└── LICENSE
```
## Methodology Overview
The pipeline consists of three main stages:

### 1. Environment Setup
Installation of dependencies and configuration of the computational environment directly within the notebook (optimized for Google Colab/Jupyter environments).

### 2. Data Processing, Model Training and Evaluation
The notebook performs:

Data loading and preprocessing

Feature engineering

Spatio-temporal aggregation

Training of tree-based regression models

Out-of-Time validation

Performance evaluation using MAE, RMSE, MAPE, and SMAPE metrics

The experimental protocol follows:

Training period: 2018–2023

Testing period: 2024–2025

This temporal separation was adopted to prevent data leakage and simulate real-world forecasting scenarios.

### 3. Results Generation
The pipeline generates:

Model comparison tables

Feature importance analysis

Prediction results

Manuscript figures

Supplementary analysis plots

### Dataset Availability
The complete dataset used in this research, including the processed and archived version, will be publicly available through Zenodo after the completion of the peer-review process.

Due to the double-blind review policy, the Zenodo repository and DOI information are intentionally omitted from this version of the repository.

After acceptance and publication, the permanent DOI and dataset access link will be added to this README.

For reproducibility during the review process, the processed Parquet dataset used for model training and generation of the reported results is temporarily available in the data/ directory.

### Reproducibility

To reproduce the experiments:

#### 1. Open the notebook:


TreeMedPriceForecast.ipynb

The notebook will reproduce:

Data preprocessing

Model training

Evaluation metrics

Generated tables

Figures used in the manuscript

#### Results
The results/ directory contains all experimental outputs.

Tables
Includes:

Performance comparison among evaluated models

Dataset characterization

Supplementary quantitative analyses

Figures
Includes:

Main manuscript figures

Feature importance plots

Temporal forecasting analysis

Supplementary figures for benchmarked algorithms

License
This project is licensed under the Apache License 2.0.
You may use, modify, and distribute this software under the terms and conditions of the Apache License 2.0.

The processed dataset will be distributed under an appropriate open data license through Zenodo after the peer-review process.

Citation
The citation information will be updated after publication.
If you use this repository or the associated dataset, please cite the final published article and the Zenodo dataset DOI.
