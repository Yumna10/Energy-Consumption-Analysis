# Energy Consumption Analysis Project  

## Overview  
This project focuses on analyzing energy consumption data to extract insights, optimize energy usage, and reduce costs. By leveraging statistical methods and data visualization, the project identifies patterns and provides actionable recommendations for energy efficiency.  

## Objectives  
- Analyze energy consumption data from network sites.  
- Evaluate the impact of regions and time on energy usage.  
- Identify low-energy-consuming cells and recommend optimization thresholds.  
- Calculate potential energy and cost savings.  

## Data Description  
1. **Energy Consumption.csv**  
   - Contains energy usage data from network sites with columns:  
     - `DateTime`  
     - `Site_id`  
     - `Cell_id`  
     - `Region`  
     - `KWH/hh` (energy consumed per half hour).  

2. **Power Demand.csv**  
   - Includes energy demand for half-hour intervals with columns:  
     - `DemandDateTime`  
     - `Demand` (categorical field: High, Normal, Low).  

3. **Demand Prices**  
   - Energy prices based on demand:  
     - High: 77.21p/kWh  
     - Normal: 19.46p/kWh  
     - Low: 6.89p/kWh  

## Methodology  
1. **Data Cleaning and Preparation**  
   - Converted date columns to datetime format.  
   - Handled duplicates and standardized column names.  
   - Detected and replaced anomalies in energy consumption data.  

2. **Exploratory Data Analysis (EDA)**  
   - Visualized energy trends across regions and time.  
   - Analyzed energy consumption distribution and demand levels.  

3. **Statistical Analysis**  
   - Used ANOVA to determine if regions significantly affect energy consumption.  
   - Applied Spearman’s correlation to evaluate the relationship between time and energy usage.  

4. **Threshold Determination**  
   - Identified low-energy-consuming cells using the 25th percentile of consumption data.  

5. **Cost Savings Analysis**  
   - Calculated potential energy and monetary savings using demand prices.  

## Key Findings  
- Significant regional differences in energy consumption.  
- Weak but statistically significant correlation between time of day and energy usage.  
- Implementing a low-energy threshold saved 13,868 KWh and 283,216 EGP.  

## Tools Used  
- Python (Pandas, Matplotlib, Seaborn, Scipy)  
- Jupyter Notebook  
- Statistical Tests (ANOVA, Spearman's correlation)  

## Results  
This analysis highlights the potential of data-driven strategies to achieve energy efficiency, reduce costs, and support sustainability goals.  

## Project Files  
- **Code**: Available in the Jupyter Notebook.  
- **Dashboard**: Interactive visualizations for energy cost analysis.  
- **Presentation**: Summary of findings and methodology.  
