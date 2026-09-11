# 🌾 Seasonal Agriculture Performance Analysis & Visualization

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-3776AB.svg)](https://seaborn.pydata.org/)
[![Internship](https://img.shields.io/badge/VOIS%20x%20EduNet-Major%20Project-orange.svg)]()

---

## 📌 Project Overview

This repository contains the **Major Data Analytics Internship Project** on **Seasonal Agriculture Performance Analysis and Visualization**, conducted under the **VOIS x EduNet Foundation** program.

Agricultural productivity and farm profitability in India are deeply linked to seasonal variations, climatic conditions, irrigation methods, and resource management. This project applies exploratory data analysis (EDA), data cleaning, statistical evaluation, bivariate & multivariate visualization, and feature engineering to a multi-farm dataset. The objective is to uncover key determinants of crop yields, water-use efficiency, disease/pest risk, and economic profitability across **Kharif**, **Rabi**, and **Zaid** seasons.

---

## 👨‍🎓 Project & Author Information

- **Student Name:** Shivam Maurya
- **College:** Arya College Of Engineering
- **Domain:** Data Analytics / Agriculture Domain Analysis
- **Program:** VOIS x EduNet Foundation Internship
- **Primary Deliverables:** 
  - `Seasonal_Agriculture_Performance_Analysis_and_Visualization.ipynb` (Full Analysis Notebook)
  - `Major_Project_Seasonal_Agriculture_Performance_Analysis.pdf` (Project Summary Report)
  - `seasonal_agriculture_performance_dataset.csv` (Dataset)

---

## 🎯 Project Objectives

1. **Data Quality & Preprocessing:** Audit dataset integrity, handle missing values via median imputation, detect outliers, and verify categorical and numerical data types.
2. **Exploratory Data Analysis (EDA):** Perform detailed **Univariate**, **Bivariate**, and **Multivariate Analysis** using Matplotlib and Seaborn.
3. **Seasonal Comparative Analysis:** Evaluate farm performance across three major agricultural seasons:
   - **Kharif** (Monsoon crops)
   - **Rabi** (Winter crops)
   - **Zaid** (Summer crops)
4. **Water Efficiency & Irrigation Impact:** Benchmark yield productivity across various irrigation techniques (**Drip**, **Sprinkler**, **Flood**, **Rainfed**) and measure **Water Efficiency ($t/1000m^3$)**.
5. **Crop-Wise Economic Analysis:** Analyze profitability ($\text{Profit\_INR}$) vs yield ($\text{Yield\_Tonnes\_Ha}$) across distinct crop types.
6. **Risk Factor Profiling:** Investigate environmental risk factors such as **Disease & Pest Risk (%)** in relation to humidity, temperature, and seasonal conditions.
7. **Strategic Recommendations:** Derive data-driven guidelines for agricultural extension services, farmers, and policy planners.

---

## 📁 Repository Structure

```
VOIS/
├── 📄 README.md                                                     # Complete Internship Project Documentation
├── 📄 LICENSE                                                       # MIT Open-Source License
├── 📊 seasonal_agriculture_performance_dataset.csv                  # Raw Agricultural Performance Dataset
├── 📓 Seasonal_Agriculture_Performance_Analysis_and_Visualization.ipynb  # Primary Python Jupyter Notebook
└── 📕 Major_Project_Seasonal_Agriculture_Performance_Analysis.pdf   # Formal Project Presentation / Report
```

---

## 📊 Dataset Description & Feature Schema

The dataset comprises comprehensive farm-level records capturing environmental parameters, resource utilization, crop varieties, and economic returns:

| Variable | Type | Description |
| :--- | :--- | :--- |
| `Farm_ID` | Identifier | Unique identification code for each farm record |
| `State` | Categorical | Geographic state location of the farm |
| `Crop` | Categorical | Crop type grown (*Sugarcane, Chilli, Maize, Rice, Wheat, Groundnut, Cotton, Pulses*) |
| `Season` | Categorical | Agricultural cropping season (*Kharif, Rabi, Zaid*) |
| `Avg_Temperature_C` | Numerical | Average seasonal temperature (°C) |
| `Rainfall_mm` | Numerical | Total seasonal rainfall received (mm) |
| `Humidity_pct` | Numerical | Relative atmospheric humidity (%) |
| `Soil_Moisture_pct` | Numerical | Soil moisture content (%) |
| `Farm_Area_Hectares` | Numerical | Total cultivated land area (Hectares) |
| `Water_Used_m3` | Numerical | Volume of irrigation water consumed ($m^3$) |
| `Irrigation_Method` | Categorical | Irrigation infrastructure (*Drip, Sprinkler, Flood, Rainfed*) |
| `Production_Tonnes` | Numerical | Total harvested crop output (Tonnes) |
| `Yield_Tonnes_Ha` | Numerical | Agricultural yield per unit area ($\text{Tonnes}/\text{Hectare}$) |
| `Profit_INR` | Numerical | Net financial profit or loss generated ($\text{INR } ₹$) |
| `Water_Efficiency_t_per_1000m3` | Derived | Crop yield generated per unit water ($\text{Tonnes} / 1000m^3$) |
| `Disease_Pest_Risk_pct` | Numerical | Estimated risk level of pest infestation/crop disease (%) |

---

## 🛠️ Technology Stack & Analytical Methods

- **Language:** Python 3.8+
- **Data Manipulation:** `pandas`, `numpy`
- **Data Visualization:** `seaborn`, `matplotlib.pyplot`
- **Statistical Analysis:** Descriptive Statistics, Median Imputation, IQR Outlier Detection, Correlation Heatmaps, Pair Plots, Groupby Aggregations.

---

## 📈 Key Findings & Insights

### 1. Seasonal Productivity & Resource Demand
- **Kharif Season** recorded the highest average yield (**5.63 tonnes/ha**) and total volume production. However, it also demanded the highest average irrigation water volume (**6,102.20 $m^3$**).
- **Zaid Season** exhibited the lowest water efficiency (**4.41 tonnes per 1,000 $m^3$**) and highest pest susceptibility.
- **Rabi Season** demonstrated consistent, moderate yield (**5.00 tonnes/ha**) with stable water utilization (**5.19 tonnes per 1,000 $m^3$**).

### 2. Crop Productivity & Profitability Disparity
- **Sugarcane** led across all crops with an average yield of **46.64 tonnes/ha** and maximum net profitability averaging **₹817,187.99**.
- **Chilli** emerged as the second most profitable crop, averaging **₹750,878.34** profit.
- **Cereal Crops (Wheat, Rice, Maize)** exhibited negative average net profits (Wheat: **-₹123,398.34**, Rice: **-₹102,213.50**, Maize: **-₹83,978.33**), underscoring high input costs and market price volatility.
- **Pulses** recorded the lowest average yield (**0.92 tonnes/ha**).

### 3. Irrigation Infrastructure Performance
- **Drip Irrigation** outperformed all other irrigation techniques, yielding an average of **6.58 tonnes/ha**.
- Performance comparison across irrigation methods:
  - **Drip:** $6.58 \text{ tonnes/ha}$
  - **Sprinkler:** $5.16 \text{ tonnes/ha}$
  - **Flood:** $4.86 \text{ tonnes/ha}$
  - **Rainfed:** $4.60 \text{ tonnes/ha}$

### 4. Disease & Pest Risk Dynamics
- **Zaid Season** suffered the highest average **Disease & Pest Risk (52.01%)**, driven by summer temperature highs and elevated pest propagation windows.

---

## 💡 Strategic Recommendations

1. **Targeted Pest Management in Zaid Season:** Implement early-warning pest surveillance, crop rotation, and bio-pesticide interventions during summer months.
2. **Expansion of Micro-Irrigation (Drip Systems):** Incentivize adoption of Drip Irrigation to maximize yield per hectare and conserve ground water reserves.
3. **Optimizing Crop Selection for Profitability:** Encourage farmers to balance food-grain production with high-value cash crops (e.g., Chilli, Sugarcane) to offset losses observed in cereal cultivation.
4. **Cost-Input Auditing for Cereal Farming:** Conduct regional evaluations on fertilizer, seed, and labor costs for Rice, Wheat, and Maize to restore farm profitability.
5. **Data-Driven Precision Agriculture:** Utilize integrated soil moisture, weather data, and water efficiency metrics for dynamic irrigation scheduling.

---

## 🚀 How to Run the Project

### Prerequisites
Ensure Python 3.8+ and Jupyter Notebook are installed on your system.

### Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.org/scriptedbyshivam/vois-x-edunet.git
   cd vois-x-edunet
   ```

2. **Install required packages:**
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. **Launch the Jupyter Notebook:**
   ```bash
   jupyter notebook Seasonal_Agriculture_Performance_Analysis_and_Visualization.ipynb
   ```

---

## 📜 License

This project is licensed under the [MIT License](LICENSE) - see the LICENSE file for full details.

---

## 🙏 Acknowledgments

- **VOIS (Vodafone Intelligent Solutions)** & **EduNet Foundation** for providing the internship platform and dataset.
- **Arya College Of Engineering** for academic support and guidance.
