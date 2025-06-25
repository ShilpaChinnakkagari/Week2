# 🌍 Supply Chain Emissions Modeling (2010–2016)

## 📑 Project Description

This project focuses on analyzing and predicting **Greenhouse Gas (GHG) emissions** from U.S. industries and commodities using supply chain data from **2010 to 2016**. The primary objective is to develop regression models that estimate the **Supply Chain Emission Factors with Margins** based on descriptive information (industry, commodity, substance) and various **data quality metrics**.

The goal is to assist policymakers, researchers, and organizations in understanding emission patterns and improving supply chain sustainability.

---

## 📦 Dataset Overview

- **Source:** [Supply Chain Greenhouse Gas Emission Factors - Data.gov](https://www.data.gov/)
- **Period Covered:** 2010–2016
- **Total Records:** 22,092
- **Categories:** Industry and Commodity based

### 🗂️ Key Features:

| Column                                         | Description                                      |
| ------------------------------------------------| -------------------------------------------------|
| Code                                            | Industry/Commodity code                          |
| Name                                            | Name of the industry or commodity                |
| Substance                                       | GHG type (e.g., CO₂, methane, nitrous oxide)     |
| Unit                                            | Measurement unit (e.g., kg/2018 USD)             |
| Supply Chain Emission Factors without Margins   | Emission factor                                  |
| Margins of Supply Chain Emission Factors        | Margin of uncertainty                            |
| Supply Chain Emission Factors with Margins      | **Target variable**                              |
| DQ ReliabilityScore                             | Reliability of the data                          |
| DQ TemporalCorrelation                          | Temporal correlation quality                     |
| DQ GeographicalCorrelation                      | Geographical correlation quality                 |
| DQ TechnologicalCorrelation                     | Technological correlation quality                |
| DQ DataCollection                               | Data collection method quality                   |
| Source                                          | Commodity or Industry                            |
| Year                                            | Year of data (2010–2016)                         |

---

## 🎯 Problem Statement

Predict **Supply Chain Emission Factors with Margins** using:

- Industry and commodity data
- GHG type (substance)
- Unit of measurement
- Data Quality (DQ) metrics

---

## 🔧 Tech Stack

- **Languages:** Python
- **Libraries:** 
  - Pandas
  - NumPy
  - Matplotlib
  - Seaborn
  - Scikit-learn
  - Joblib

---

## 🚀 Project Workflow

### 1️⃣ Data Preprocessing
- Handle missing values
- Drop irrelevant columns
- Encode categorical variables
- Normalize numerical features

### 2️⃣ Exploratory Data Analysis (EDA)
- Understand data distribution
- Correlation analysis
- Visualization of emissions across years and industries

### 3️⃣ Model Building
Models Used:
- Linear Regression
- Random Forest Regressor

### 4️⃣ Model Evaluation
- **R² Score**
- **RMSE (Root Mean Squared Error)**
- **MAE (Mean Absolute Error)**

### 5️⃣ Hyperparameter Tuning
- GridSearchCV for Random Forest optimization

### 6️⃣ Model Comparison
- Evaluate performance
- Select best-performing model

---

## 📂 File Structure

├── data/
│ └── SupplyChainEmissionFactorsforUSIndustriesCommodities.xlsx
├── notebooks/
│ └── Supply_Chain_Emissions_Modeling.ipynb
├── models/
│ └── final_model.pkl
├── README.md
├── requirements.txt
└── LICENSE
