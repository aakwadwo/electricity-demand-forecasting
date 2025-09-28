# electricity-demand-forecasting
Forecast electricity demand for Ghana &amp; Nigeria using WDI data.
# Electricity Demand Forecasting (Ghana & Nigeria)

This project forecasts electricity demand for Ghana and Nigeria using World Bank WDI data.

## Methodology
- Data sourced from **World Bank WDI** ("Electric power consumption (kWh per capita)").
- Cleaned dataset to extract Ghana and Nigeria demand across years.
- Feature engineering: created lag features (1–5 years), rolling averages, and growth rates.
- Model: Linear Regression with lagged features.
- Achieved **Mean Squared Error (MSE) = 14.12** on test data.
- Forecasts future electricity demand up to any input year.

## Forecasting Example
```python
forecast("Ghana", 2030)
forecast("Nigeria", 2030)