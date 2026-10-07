# Airplane Crashes and Fatalities Analysis (1908 – Present) - EDA

This repository contains an extensive **Exploratory Data Analysis (EDA)** project on historical aviation accidents from 1908 to modern times. The main objective of this study is to uncover patterns, trends, and key insights related to air safety, fatality rates, operators, aircraft types, and historical accident locations.

---

## 📌 Project Overview

Aviation safety has evolved significantly over the past century. By analyzing over 5,000 recorded crash events, this project explores:
- Historical trends in aviation accidents and fatality counts over time.
- Correlation between total passengers aboard and fatality rates.
- Most frequent crash locations, operators, and aircraft types.
- Text analysis and feature extraction from crash summaries and dates (e.g., month/year trends, aircraft manufacturers).

---

## 📊 Dataset Description

The dataset used in this analysis is `Airplane_Crashes_and_Fatalities_Since_1908.csv`, containing **5,268 records** and **13 primary attributes**:

| Column Name | Description |
| :--- | :--- |
| **Date** | Date of the accident (MM/DD/YYYY) |
| **Time** | Local time of the accident |
| **Location** | Geographical location of the accident |
| **Operator** | Airline or military unit operating the flight |
| **Flight #** | Flight number (if applicable) |
| **Route** | Flight path/destination details |
| **Type** | Aircraft model/type |
| **Registration** | Aircraft registration code |
| **cn/In** | Construction or serial number |
| **Aboard** | Total number of people on board |
| **Fatalities** | Total number of fatalities on board |
| **Ground** | Number of fatalities on the ground |
| **Summary** | Brief narrative describing the crash incident |

---

## 🛠️ Key Features & Methodology

1. **Data Cleaning & Preprocessing:**
   - Handled missing values across key categorical and numerical attributes (`Location`, `Operator`, `Aboard`, `Fatalities`, `Time`, etc.).
   - Converted dates into structured datetime objects and extracted `Month` and `Year` features.
   - Extracted primary manufacturer names from the `Type` field.

2. **Exploratory Data Analysis (EDA):**
   - Statistical summaries and correlation analysis between `Aboard`, `Fatalities`, and `Ground` figures.
   - Geographical and operator-level frequency distributions.
   - Time-series and seasonal analysis of air crashes.

3. **Data Profiling & Visualization:**
   - Interactive and static charts utilizing **Plotly**, **Seaborn**, and **Matplotlib**.
   - Automated profiling reports using `ydata-profiling`.
   - Text analytics leveraging **NLTK**.

---

## 🧰 Tech Stack & Libraries

- **Language:** Python 3.x
- **Data Manipulation:** `pandas`, `numpy`
- **Visualization:** `matplotlib`, `seaborn`, `plotly`
- **Statistical Analysis:** `scipy`, `statsmodels`
- **NLP / Text Processing:** `nltk`
- **Automated Reporting:** `ydata-profiling`
