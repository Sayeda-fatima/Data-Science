# Website A/B Testing Analysis and Hypothesis Testing

This project focuses on the A/B testing data. The test was conducted to optimize the website design, splitting the traffic between control and treatment groups. The control group was shown a "sign up" button in red, while the treatment group was shown it in green.

## Project Overview
The following tasks were completed in this project:
1. **Data Import and Exploration**: Data was loaded from the **ABTest** sheet into a Pandas DataFrame (`abtest`). Basic exploratory analysis was performed to understand the data.
2. **Time-Series Visualization**: A time-series visualization was created with **Date** on the x-axis and **Total Number of Clicks** on the y-axis. Separate trendlines for each device type were generated to find the best-performing device in terms of total clicks.
3. **Sample Size Calculation**: The required sample size for the A/B test was calculated using a Minimum Detectable Effect (MDE) of 3%, an alpha of 95%, and a statistical power of 80%.
4. **Hypothesis Testing Function**: A function was written to conduct hypothesis testing, comparing control and treatment group conversion rates at different confidence levels (90%, 95%, 99%). The function outputs one of three results: 
   - "Experiment Group is Better"
   - "Control Group is Better"
   - "Indeterminate"
5. **Results Interpretation**: The function was applied to the data to assess which variation of the website performed better.

## Dataset Description
The **ABTest** dataset contains the following key columns:
- **Date**: The date of the observation.
- **Device Type**: The type of device used by visitors (e.g., Mobile, Desktop).
- **Control Group Visitors**: Number of visitors in the control group.
- **Control Group Clicks**: Number of clicks in the control group.
- **Treatment Group Visitors**: Number of visitors in the treatment group.
- **Treatment Group Clicks**: Number of clicks in the treatment group.
