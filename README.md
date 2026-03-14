# Customer Personality Marketing ML

![Project Header](assets/Project%20Header.jpg)

A machine learning solution for customer segmentation and personality analysis to boost marketing campaign effectiveness.

## Project Overview

End-to-end data science project that analyzes customer demographics, spending behavior, and engagement metrics to identify distinct customer segments. Includes comprehensive EDA, preprocessing pipelines, K-means clustering, and an interactive Streamlit dashboard for segment prediction and business recommendations.

## Key Results

- **Customer Segments**: 4 distinct clusters identified
- **Model Algorithm**: K-means Clustering with PCA (85% variance retention)
- **Cluster Distribution**:
  - Low-Engagement Customers: 27.78%
  - Mid-Tier Active Customers: 27.19%
  - Premium Engaged Customers: 28.37%
  - High-Browse Low-Convert: 16.66%
- **Campaign Optimization**: Tailored recommendations for each segment to improve response rates

## Project Structure

```
├── assets/                 # Project images and media
├── data/                   # Raw and processed datasets
│   ├── marketing_campaign_data.csv
│   ├── pca_input_kmeans.csv
│   └── cluster_summary_statistics.xlsx
├── models/                 # Trained model artifacts
│   ├── kmeans_model.joblib
│   └── scalers.joblib
├── tasks/                  # Original bootcamp assignment materials
│   ├── Task 1 - EDA/
│   ├── Task 2 - Data Cleaning & Preprocessing/
│   └── Task 3 - Data Modeling/
├── utils/                  # Reusable preprocessing and ML functions
│   ├── preprocessing.py
│   ├── feature_definitions.py
│   └── cluster_interpretations.py
├── main.py                 # Streamlit application
├── notebook.ipynb          # EDA and model training notebook
├── pyproject.toml          # Project dependencies (uv/pip)
├── requirements.txt        # Pip-compatible dependencies
└── README.md              # Project documentation
```

## Quick Start

### Prerequisites

- Python 3.12+
- uv (recommended) or pip

### Installation

```bash
# Clone repository
git clone https://github.com/mcikalmerdeka/customer-personality-marketing-ml.git
cd customer-personality-marketing-ml

# Create virtual environment
python -m venv .venv

# Activate virtual environment
# On Windows:
.venv\Scripts\activate
# On macOS/Linux:
source .venv/bin/activate

# Install dependencies (using pip)
pip install -r requirements.txt

# Or using uv (faster alternative)
uv sync
```

### Run the App

```bash
streamlit run main.py
```

Access the app at `http://localhost:8501`

## Features

- **Data Input Options**: Upload custom CSV or use built-in source data
- **Interactive Preprocessing**: Step-by-step data cleaning with customizable parameters
  - Data type conversion
  - Missing value imputation
  - Outlier handling
  - Feature engineering
  - Categorical encoding
  - Feature scaling
- **PCA Visualization**: 2D cluster visualization using Principal Component Analysis
- **Cluster Statistics**: Detailed segment analysis with key metrics
- **Business Recommendations**: Tailored strategies for each customer segment
- **New Customer Prediction**: Predict segment membership for new customer data
- **Data Dictionary**: Comprehensive feature explanations and definitions

## Technical Stack

- Python 3.12+
- scikit-learn (K-means clustering, PCA, preprocessing)
- pandas, numpy (data processing)
- matplotlib, seaborn (visualization)
- Streamlit (web application)
- joblib (model serialization)
- uv (dependency management)

## Business Problem

A product-selling company needed to improve marketing campaign effectiveness and develop targeted strategies for different customer types. The solution segments customers based on demographics, purchasing behavior, and campaign responsiveness, enabling the Marketing team to optimize campaigns and the Sales team to personalize their approach.

### Problem Statements

1. **Customer Segmentation**: How can we group customers into meaningful segments based on their characteristics and behaviors?
2. **Campaign Optimization**: How can we tailor marketing campaigns to different customer segments to improve response rates and conversion?

### Assumptions & Scope

- The data provided is accurate and representative of the customer base
- Past behavior (purchases, website visits, campaign responses) is indicative of future behavior
- Demographic factors (age, education, marital status) influence purchasing decisions
- Customer complaints within the last 2 years significantly impact their relationship with the company
- The recency of a customer's last purchase is related to their likelihood of future purchases
- Customers who engage more frequently (website visits, purchases) are more valuable to the company

## Try the Live App

[Streamlit Cloud Deployment](https://customer-personality-marketing-ml-wxgaitu6nq6qdb94c8xzdq.streamlit.app/)

## Project Background

This project originally came from an assignment after a data science bootcamp program. The **`tasks`** folder contains the original assignment instructions, presentations, and deliverables. The project has been further developed with additional knowledge from work experience, online courses, and best practices in MLOps and software engineering.

## Author

**Muhammad Cikal Merdeka** | Data Analyst/Data Scientist

- [GitHub](https://github.com/mcikalmerdeka)
- [LinkedIn](https://www.linkedin.com/in/mcikalmerdeka)
