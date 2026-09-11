# 🌾 Seasonal Agriculture Performance Analysis & Visualization

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-3776AB.svg)](https://seaborn.pydata.org/)
[![Status](https://img.shields.io/badge/Status-Completed-success.svg)](#)

---

## 📌 Project Overview

This repository contains the **Major Data Analytics Internship Project** on **Seasonal Agriculture Performance Analysis and Visualization**, conducted as part of the **VOIS x EduNet Foundation Internship Program**.

Agricultural productivity and farm profitability in India are heavily influenced by seasonal shifts, weather metrics (temperature, rainfall, humidity, soil moisture), irrigation infrastructure, and resource efficiency. This project performs end-to-end Exploratory Data Analysis (EDA), data preprocessing, missing value imputation, statistical modeling, and data visualization on a multi-farm dataset to evaluate crop yields, water-use efficiency, disease/pest risk, and financial returns across **Kharif**, **Rabi**, and **Zaid** cropping seasons.

---

## 👨‍🎓 Project & Author Details

| Attribute | Details |
| :--- | :--- |
| **Student Name** | Shivam Maurya |
| **Institution** | Arya College Of Engineering |
| **Domain** | Data Analytics / Agricultural Domain Analytics |
| **Program** | VOIS x EduNet Foundation Internship |
| **Deliverables** | Primary Notebook (`.ipynb`), Reports (`.pdf`), Presentation (`.pptx`), Dataset (`.csv`) |

---

## 🎯 Key Objectives

1. **Data Cleaning & Quality Audit:** Check for missing values, duplicate records, outliers, and data type consistency across all features.
2. **Exploratory Data Analysis (EDA):** Perform **Univariate**, **Bivariate**, and **Multivariate Analysis** to reveal hidden patterns.
3. **Seasonal Performance Evaluation:** Compare productivity and resource demands across **Kharif** (Monsoon), **Rabi** (Winter), and **Zaid** (Summer) seasons.
4. **Irrigation & Water Efficiency Benchmarking:** Evaluate yield outcomes across irrigation methods (**Drip**, **Sprinkler**, **Flood**, **Rainfed**) and measure water efficiency ($\text{Tonnes} / 1000m^3$).
5. **Crop Profitability & Risk Profiling:** Analyze cost vs. profitability across 8 major crops and measure **Disease & Pest Risk (%)**.
6. **Actionable Business Recommendations:** Provide evidence-based recommendations for farmers, agricultural extension workers, and policy planners.

---

## 📁 Repository Structure

```
VOIS/
├── 📄 README.md                                                        # Comprehensive Project Documentation
├── 📄 LICENSE                                                          # MIT Open-Source License
├── 📊 seasonal_agriculture_performance_dataset.csv                     # Raw Agricultural Dataset
├── 📓 Seasonal_Agriculture_Performance_Analysis_and_Visualization.ipynb # Primary Analysis & EDA Notebook
├── 📕 Major_Project_Seasonal_Agriculture_Performance_Analysis.pdf      # Executive Summary Report
├── 📕 Data_Visualization_VOIS.pdf                                      # Complete Visual Analytics Report
└── 📙 VOIS_Major_Project_PPT_Submission.pptx                           # Major Project Slide Deck Presentation
```

---

## 📊 Dataset Schema & Feature Description

The dataset contains farm-level agricultural metrics capturing environmental parameters, land size, resource usage, crop details, and economic outcomes:

| Feature Name | Category | Unit / Format | Description |
| :--- | :--- | :--- | :--- |
| `Farm_ID` | Identifier | String | Unique identification code for each farm record |
| `State` | Demographics | String | Indian State location of the farm |
| `Crop` | Categorical | String | Type of crop grown (*Sugarcane, Chilli, Maize, Rice, Wheat, Groundnut, Cotton, Pulses*) |
| `Season` | Categorical | String | Cropping season (*Kharif, Rabi, Zaid*) |
| `Avg_Temperature_C` | Environmental | °C | Average seasonal temperature |
| `Rainfall_mm` | Environmental | mm | Total seasonal rainfall received |
| `Humidity_pct` | Environmental | % | Average relative humidity |
| `Soil_Moisture_pct` | Environmental | % | Average soil moisture percentage |
| `Farm_Area_Hectares` | Resource | Hectares | Cultivated land area |
| `Water_Used_m3` | Resource | $m^3$ | Total volume of irrigation water consumed |
| `Irrigation_Method` | Infrastructure | String | Method used (*Drip, Sprinkler, Flood, Rainfed*) |
| `Production_Tonnes` | Output | Tonnes | Total harvested agricultural output |
| `Yield_Tonnes_Ha` | Output Metric | Tonnes/Ha | Crop yield per hectare |
| `Profit_INR` | Economic Metric | INR (₹) | Net financial profit or loss generated |
| `Water_Efficiency_t_per_1000m3` | Derived Metric | Tonnes/$1000m^3$ | Yield produced per unit of irrigation water |
| `Disease_Pest_Risk_pct` | Risk Metric | % | Estimated pest infestation and disease risk |

---

## 🛠️ Tech Stack & Analytical Pipeline

- **Programming Language:** Python 3.8+
- **Data Manipulation:** `pandas`, `numpy`
- **Data Visualization:** `seaborn`, `matplotlib.pyplot`
- **Statistical Methods:** IQR Outlier Analysis, Median Imputation, Correlation Matrix Heatmaps, Groupby Aggregations, Pairplots.

---

## 📈 Key Findings & Analytical Insights

### 1. Seasonal Performance Breakdown
- **Kharif Season:** Highest average yield (**5.63 tonnes/ha**) and maximum production volume, but requires the highest average water consumption (**6,102.20 $m^3$**).
- **Zaid Season:** Lowest water efficiency (**4.41 tonnes per 1,000 $m^3$**) and highest pest risk.
- **Rabi Season:** Stable yield (**5.00 tonnes/ha**) and reliable water efficiency (**5.19 tonnes per 1,000 $m^3$**).

### 2. Crop Productivity vs Profitability
- **Sugarcane:** Highest average yield (**46.64 tonnes/ha**) and highest net profit (**₹8,17,187.99**).
- **Chilli:** Second highest profitability (**₹7,50,878.34**).
- **Cereal Crops (Wheat, Rice, Maize):** Recorded negative average net profits (Wheat: **-₹1,23,398.34**, Rice: **-₹1,02,213.50**, Maize: **-₹83,978.33**) due to high input costs and market pricing pressure.
- **Pulses:** Lowest average yield (**0.92 tonnes/ha**).

### 3. Irrigation Method Benchmarking
- **Drip Irrigation:** Highest average yield (**6.58 tonnes/ha**).
- **Yield Comparison:** Drip (**6.58 t/ha**) > Sprinkler (**5.16 t/ha**) > Flood (**4.86 t/ha**) > Rainfed (**4.60 t/ha**).

### 4. Environmental Risk Factors
- **Zaid Season** has the highest average **Disease & Pest Risk (52.01%)**, linked to summer heat and humidity fluctuations.

---

## 💡 Strategic Recommendations

1. **Integrated Pest Management (Zaid Season):** Implement proactive pest surveillance and crop protection during Zaid.
2. **Promote Drip Irrigation:** Incentivize Drip systems to enhance water productivity and increase yield per hectare.
3. **Crop Diversification:** Encourage farmers growing low-margin cereals to diversify into high-value crops like Chilli and Sugarcane.
4. **Input Cost Optimization:** Audit input costs (fertilizer, seeds, diesel/electricity) for Rice and Wheat to restore farm profitability.
5. **Data-Driven Scheduling:** Use soil moisture and weather metrics for smart irrigation planning.

---

## 🚀 Getting Started

### Prerequisites
Make sure Python 3.8+ is installed.

### Setup & Execution
1. **Clone the Repository:**
   ```bash
   git clone https://github.org/scriptedbyshivam/vois-x-edunet.git
   cd vois-x-edunet
   ```

2. **Install Required Packages:**
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. **Run the Notebook:**
   ```bash
   jupyter notebook Seasonal_Agriculture_Performance_Analysis_and_Visualization.ipynb
   ```

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙏 Acknowledgments

- **VOIS (Vodafone Intelligent Solutions)** & **EduNet Foundation** for the internship opportunity and dataset.
- **Arya College Of Engineering** for academic support.
