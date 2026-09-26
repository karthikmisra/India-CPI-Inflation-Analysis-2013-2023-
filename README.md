# India-CPI-Inflation-Analysis-2013-2023-
An Excel-basedanalysis of India's CPI (2013-2023), exploring inflation drivers, COVID-19 economic shocks, and global oil price correlations.
# India CPI & Macroeconomic Inflation Analysis (2013–2023)

## 📌 Executive Summary
This project provides an end-to-end macroeconomic analysis of India's Consumer Price Index (CPI) across Rural and Urban sectors from 2013 to 2023. By leveraging advanced Excel techniques, this case study uncovers the core drivers of retail inflation, measures the economic shock of the COVID-19 pandemic, and quantifies the cascading effects of global crude oil price fluctuations on domestic household budgets.

---

## 🎯 Business Problem & Core Objectives
The objective of this analysis is to decode complex economic indicators into actionable insights by solving six specific macroeconomic problem statements:
1. **Basket Contribution:** Calculate the weight and contribution of broader commodity categories to the latest CPI calculation.
2. **Long-Term Trend Analysis:** Identify the peak Year-over-Year (YoY) inflation year since 2017 and correlate it with global geopolitical events.
3. **Food Volatility:** Track Month-on-Month (MoM) food inflation over a 12-month period and isolate the single largest absolute commodity driver.
4. **Pandemic Economic Shock:** Measure the immediate inflationary impact of the March 2020 COVID-19 lockdowns across distinct essential and non-essential sectors.
5. **Global Crude Oil Impact:** Use internal transport indexes as a proxy to calculate the correlation between oil shocks and cascading service inflation.
6. **Inflation Calculator Build:** Develop a dynamic, rolling calculator for both Monthly and Annual inflation rates.

---

## 🗂 Dataset Overview
* **Data Source:** Ministry of Statistics and Programme Implementation (MoSPI) / Government of India CPI Data.
* **Timeline:** January 2013 to May 2023.
* **Scope:** `Rural+Urban` combined sector data.
* **Key Dimensions:** 
  * 24 distinct sub-categories (e.g., Cereals, Spices, Clothing, Housing, Health, Transport).
  * Pre-aggregated macro-buckets (e.g., General Index, Food and Beverages, Miscellaneous).

---

## ⚙️ Technical Excel & Analytical Implementations
Designed as a comprehensive showcase of foundational data analytics and spreadsheet modeling skills:
* **Statistical Functions:** Utilized the `=CORREL` function to mathematically prove the relationship between fuel price shocks and the inflation of downstream logistics and household services.
* **Dynamic Time-Series Logic:** Built rolling 12-month Annual Inflation calculators using relative row referencing (`= (Current - Shift 12) / Shift 12`) dependent on chronological custom sorting.
* **Pivot Table Aggregation:** Deployed Pivot Tables configured to Average (rather than Sum) to calculate clean annual baseline indexes, naturally bypassing missing pandemic data (April/May 2020).
* **Data Hygiene & Preprocessing:** Filtered and isolated specific 12-month trailing windows to prevent data leakage during Month-on-Month (MoM) evaluations.
* **Visual Formatting:** Applied Top/Bottom conditional formatting rules and multi-color heat scales to instantly highlight peak volatility months and primary absolute contributors.

---

## 📊 Strategic Findings & Analytical Breakdown

### 1. CPI Basket Weighting (May 2023)
* **Food is the Primary Driver:** The broader Food category overwhelmingly dictates Indian inflation, contributing **51.73%** to the total index calculation. 
* **Secondary Drivers:** Miscellaneous services (17.81%) and Clothing & Footwear (8.92%) represent the next largest consumer burdens.

### 2. Macro Trend & Geopolitical Impact
* **Peak Inflation Year:** Year-over-Year inflation peaked at **6.62% in 2022**.
* **Driver:** This spike directly aligns with the outbreak of the Russia-Ukraine war, which triggered massive global supply chain disruptions and commodities shocks (specifically in crude oil, edible oils, and fertilizers).

### 3. Food Price Volatility (Trailing 12-Months: Jun '22 – May '23)
* **Highs and Lows:** Food inflation experienced severe swings, peaking at **+1.01% MoM** in October 2022 and dropping to a deflationary **-1.35% MoM** in December 2022.
* **Absolute Contributor:** Comparing May 2022 to May 2023, **Spices** saw an unprecedented absolute index increase of **+33.10 points**, acting as the single largest upward driver in the food bucket, followed by Cereals (+19.60).

### 4. The COVID-19 Economic Shock (Mar '20 Lockdown)
Comparing the 12 months pre-lockdown (Mar '19–Feb '20) to the 12 months post-lockdown (Apr '20–Mar '21):
* **Supply Shocks:** Overall General Inflation rose from 4.83% to 5.66%, driven heavily by Food inflation jumping from 5.82% to 6.99% due to supply chain halts and panic buying.
* **Demand Destruction:** Conversely, Health inflation cooled (7.20% down to 4.68%) as elective procedures halted, and Household Goods inflation dropped (3.72% to 2.45%) as non-essential spending evaporated.

### 5. Cascading Oil Price Correlations (2021–2023)
* **The Proxy:** Using "Transport and Communication MoM" as the internal proxy for imported crude oil prices.
* **The Ripple Effect:** The **Miscellaneous** category (encompassing local logistics, household services, and goods) displayed a massive **0.81 positive correlation** with Transport. This quantitatively proves that fuel price shocks are immediately passed down to the consumer in the form of more expensive daily services and goods.

---

## 📁 Repository Structure
```text
├── data/
│   └── All_India_Index_Upto_April23 (1).csv      # Raw dataset
├── notebooks/
│   └── India_CPI_Analysis_Workbook.xlsx          # Analyzed Excel file with all formulas & pivot models
├── visuals/
│   └── YoY_Inflation_Trend_Graph.png             # Line graph demonstrating the 2022 inflation peak
├── docs/
│   └── Problem_Statements.pdf                    # Original case study questions and parameters
└── README.md                                     # Project documentation and summary
