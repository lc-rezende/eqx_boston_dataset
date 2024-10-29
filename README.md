# EQX Crime Analysis - Boston Crime Dataset

> **Disclaimer**: This project is a case study analysis conducted for exploratory and educational purposes. The findings and forecasts presented here are based on historical data and do not reflect real-time conditions.

This project provides an exploratory data analysis (EDA), clustering, and forecasting of crime data in Boston, with the primary aim of uncovering patterns and trends to assist with crime prevention and resource allocation. 

## Dataset
The dataset includes crime reports from 2011 to 2015, containing details on crime types, dates, locations, arrests, and domestic-related incidents. Each data entry also specifies geolocation coordinates (latitude and longitude), facilitating spatial analysis.

## Key Steps and Analysis

### 1. Data Cleaning and Preparation
- **Data Transformation**: Dates were standardized, unnecessary columns were dropped, and categorical variables were created for `Primary Type`, `Description`, and `Location Description` to optimize analysis.
- **Handling Missing Data**: Missing geolocation coordinates and district data were removed to maintain accuracy.

### 2. Exploratory Data Analysis (EDA)
- **Crime Trends Over Time**:
  - Monthly and daily aggregations revealed a consistent trend in crime reports, with peaks and valleys that suggest seasonal and day-of-week variations.
  - Notably, higher crime volumes were observed on Fridays and Saturdays, suggesting a weekend correlation.

- **Crime Distribution by Type**:
  - **Top Crime Types**: Theft, battery, narcotics, and criminal damage were the most frequent offenses.
  - **Location Insights**: Streets, residences, and sidewalks were the most common crime locations, underscoring high-risk public spaces.

### 3. Clustering Analysis
Using hierarchical and k-means clustering techniques:
- **Crime Type by Day of Week**: Clustered data highlighted days with increased specific crimes, such as more narcotics-related incidents midweek.
- **Location Clustering**: High-frequency locations like streets and residential areas were grouped, revealing hotspots for specific crime types, which can aid targeted patrolling.

### 4. Forecasting Crime Trends
A time-series forecasting model was built using Facebook Prophet to predict crime volumes for upcoming months in different districts.
- **6-Month and 12-Month Forecasts**: Projections indicated slight increases in crime volume for certain areas, providing actionable insights for future resource deployment and preventive strategies.

## Key Insights
- **Temporal Patterns**: Crime frequency varies by day of the week and month, with notable spikes during weekends.
- **Location-Specific Risks**: Streets and residential areas are hotspots, which may benefit from increased monitoring or community safety programs.
- **Forecasting for Proactive Action**: Forecasted crime rates provide valuable insights for law enforcement to pre-emptively allocate resources to districts with expected crime increases.

## Tools and Libraries
- **Data Processing**: `Pandas`, `NumPy`
- **Visualization**: `Matplotlib`, `Seaborn`
- **Clustering**: `Scikit-Learn`'s KMeans and AgglomerativeClustering
- **Forecasting**: `Facebook Prophet`

## Conclusion
This analysis presents critical findings on crime trends in Boston, emphasizing high-risk areas, temporal patterns, and forecasted crime activity. The insights derived here support proactive policing strategies and highlight the potential for data-driven decision-making in urban crime management.

## Repository Structure
- **Eqx Crime Analysis.ipynb**: Contains the code for data processing, EDA, clustering, and forecasting.
- **README.md**: (Current file) Overview of the project, methodology, and insights.

---

For questions or to connect further, feel free to reach out via [LinkedIn](https://www.linkedin.com/in/lucascrezende).
