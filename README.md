# MKS Instruments: Strategic Marketing Data Pipeline

This repository features an automated data validation and predictive analytics pipeline specifically designed for **MKS Instruments'** B2B strategic marketing scenarios. It demonstrates a complete MLOps workflow—from raw data quality assurance to lead propensity modeling.

## 📍 Repository Structure & File Location

To ensure a clean production environment, the core logic is organized as follows:

* **Main Script**: `TFDV_Labs/mks_strategic_marketing_tfdv.py`
    * Integrates synthetic B2B data generation, business logic validation, and a TensorFlow-based neural network.
* **Environment Configuration**: `.gitignore`
    * Strictly configured to exclude `.venv` and temporary cache files, ensuring only source code is version-controlled.

## 🚀 Key Features

### 1. Automated Data Quality Assurance (QA)
Tailored for MKS's core business segments (Semiconductor, Photonics, etc.), the pipeline automatically intercepts:
* **Financial Anomalies**: Detecting negative or outlier revenue figures.
* **Segment Drift**: Ensuring input data aligns with target B2B industry categories.

### 2. Customer Propensity Modeling
Utilizes a **TensorFlow/Keras** Multi-Layer Perceptron (MLP) to predict the probability of high-value equipment upgrades based on:
* Equipment service life (Age).
* Historical purchasing cycles.
* Marketing engagement scores.

## 🛠️ Getting Started

1.  **Activate Environment**:
    ```powershell
    .\.venv\Scripts\activate
    ```
2.  **Install Dependencies**:
    ```powershell
    pip install tensorflow pandas scikit-learn
    ```
3.  **Run the Pipeline**:
    ```powershell
    python TFDV_Labs/mks_strategic_marketing_tfdv.py
    ```

## 📈 Business Impact
* **Decision Integrity**: Minimizes risk by preventing "garbage-in, garbage-out" scenarios in strategic planning.
* **Sales Efficiency**: Automates the identification of high-potential leads, allowing the sales team to focus on customers with the highest upgrade propensity.
