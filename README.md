# Forecasting Chocolate Production in Australia

This project is part of the **Supply Chain Analytics** course and focuses on **forecasting quarterly production of chocolate confectionery** in Australia using various time series methods.

---

## Objective

To compare multiple forecasting models and recommend the best-fitting approach for predicting future production patterns in the chocolate industry.

---

## Methods Used

We applied **9 forecasting models**:

1. Linear Trend  
2. Quadratic Trend  
3. Exponential Growth  
4. Linear with Seasonality (Dummy Variables)  
5. Quadratic with Seasonality  
6. Exponential with Seasonality  
7. Linear using Deseasonalized Sales (MA12)  
8. Quadratic using Deseasonalized Sales  
9. Exponential using Deseasonalized Sales  

Each method was evaluated based on its **Mean Absolute Deviation (MAD)** and **forecast curve accuracy**.

---

## Insights

- **Quadratic models** better captured curve behavior during trend shifts  
- The **seasonal pattern changed over time**, with the peak moving from Q2 to Q4  
- **Manual adjustment** was used to better align forecast with observed seasonality in recent years  
- Using the **entire time series added noise** — optimal results came from trimming early years

---

## Files

- `data/Quarterly_Chocolate_Solution.xlsx` — Raw and calculated forecasts with blue comments  
- `data/DataSet_Chocolate.docx` — Dataset description and task instruction  
- `analysis/chocolate_forecasting_summary.md` — Method comparisons and modeling logic

---

## Learning Outcomes

- Time series forecasting for supply chain  
- Deseasonalization using moving average (MA12)  
- Impact of time range on forecast accuracy  
- Visual interpretation of trend shifts

---

## Tools Used

- Excel (formulas, dummy variables, MA12 smoothing)  
- Trend fitting + MAD calculation  
- Manual visual adjustment of forecast where models underperformed

---

This repository demonstrates forecasting techniques for supply chain decision-making in FMCG (fast-moving consumer goods) sectors.
