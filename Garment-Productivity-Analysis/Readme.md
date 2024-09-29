# Garment Worker Productivity Analysis and Forecasting

This project analyzes and forecasts the productivity of garment workers over a span of 70 days based on the WorkerFunnel dataset. The dataset includes key features like Date, Department, Targeted Productivity, Overtime, Number of Workers, Actual Productivity, and Quarter.

## Project Overview
The project is divided into several key tasks:
1. **Target Achieved Classification**: A new column named "Target Achieved" was created, indicating if the actual productivity exceeded the targeted productivity ("Yes") or not ("No").
2. **Visualization**: Grouped bar graphs were generated to visualize the productivity performance across different quarters.
3. **Forecasting**: Two models, ARIMA and Rolling Averages, were used to forecast actual productivity for the next four quarters.
4. **Evaluation Metrics**: The models were compared using Mean Absolute Percentage Error (MAPE) and Mean Squared Error (MSE) as evaluation criteria.

## Dataset Description
The WorkerFunnel dataset consists of the following columns:
- **Date**: Date of the observation in MM-DD-YYYY format.
- **Quarter**: The quarter of the month the observation falls into.
- **Department**: The department associated with the productivity report.
- **Targeted Productivity**: The expected productivity for the department/team on the given day.
- **Overtime**: The amount of overtime in minutes.
- **No. of Workers**: The number of workers involved.
- **Actual Productivity**: The actual productivity delivered as a percentage (ranging from 0 to 1).
- **Target Achieved**: A new column indicating whether the actual productivity met or exceeded the targeted productivity ("Yes"/"No").

## Visualizations
### Grouped Bar Graphs
Grouped bar graphs show the level of target achievement ("Yes" or "No") at quarterly intervals, providing insights into department performance.

### Forecasting
Forecasts for the next four quarters of actual productivity were made using:
- **ARIMA (AutoRegressive Integrated Moving Average)**
- **Rolling Averages**

The forecasts are plotted in separate line graphs for comparison.

## Evaluation Criteria
The models were evaluated using the following metrics:
1. **Mean Absolute Percentage Error (MAPE)**
2. **Mean Squared Error (MSE)**

Additional evaluation criteria include R-squared and RMSE, which are optional but provide further insight into model performance.
