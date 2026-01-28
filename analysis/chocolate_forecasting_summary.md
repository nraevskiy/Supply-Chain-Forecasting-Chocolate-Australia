# Chocolate Forecasting – Model Comparison Summary

## Objective

Compare 9 different forecasting models on quarterly chocolate production to find the best fit for current industry patterns.

---

## Key Observations

- Linear model underfit the data due to curve shifts  
- Exponential with dummy variables **fit seasonality better**, but overfit older peaks  
- Deseasonalized models using MA12 gave smoother, reliable results

---

## Challenge

A **seasonal shift** occurred:
- Past: Peaks in Q2  
- Now: Peaks in Q4  

Using older data introduced noise → Solution: start from **mid-series** for more accurate modeling.

---

## Final Recommendation

Use **Quadratic with Deseasonalized Sales (MA12)** with manual adjustment for visual accuracy in peaks/valleys.

This provided the lowest MAD and the most intuitive trend prediction for supply chain planning.

---

## MAD Comparison (Example)

| Model                         | MAD      |
|------------------------------|----------|
| Linear                       | 105.2    |
| Quadratic                    | 92.3     |
| Exponential                  | 96.4     |
| Quadratic + Dummy Vars       | 80.1     |
| Deseasonalized (Quadratic)   | **75.8** ✅ |

