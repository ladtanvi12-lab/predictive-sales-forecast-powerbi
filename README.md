Intern ID : CITS4956
FULL NAME : TANVI SUDESH LAD
NO. OF WEEKS : 4
PROJECT NAME : PREDICTIVE SALES FORECAST
PROJECT SCOPE : "Develop a Power BI dashboard to analyze 2014-2017 US Superstore sales and forecast next 6 months using interactive visuals and native time series forecasting."

# Project Title
Predictive Sales Forecast : 6-Months Forecast Dashboard using Power BI

## Brief One Line Summary
An interactive Power BI dashboard that analyzes 4 years of Superstore sales data and predicts future sales for the next 6 months with 95% confidence intervals.

## Overview
This project transforms raw Superstore transactional data into actionable business intelligence. The dashboard provides real-time KPIs, trend analysis, regional performance, and built-in time series forecasting to help stakeholders make data-driven inventory and sales decisions. It replaces manual Excel reports with automated, interactive visualizations that update with a single click.

## Problem Statement
Businesses struggle with inaccurate sales forecasting using static Excel reports, leading to two major issues: 
1. **Stockouts** during high-demand periods due to underestimation 
2. **Excess inventory** and blocked capital due to overestimation 
Manual analysis also lacks interactivity, making it difficult to drill down by Region, Segment, or Category for targeted decision-making.

## Dataset
- **Source**: Superstore Sales Dataset from Kaggle
- **Size**: 9,994 rows × 21 columns  
- **Period**: January 2014 - December 2017
- **Key Columns**: Order ID, Order Date, Ship Date, Segment, Category, Sub-Category, Sales, Profit, Discount, Region, State
- **Location**: `/superstore_cleaned_data/Superstore_Cleaned.xlsx`

## Tools and Technologies
- **BI Tool**: Microsoft Power BI Desktop
- **Data Cleaning**: Power Query Editor
- **Data Modeling**: DAX - Data Analysis Expressions
- **Forecasting**: Power BI Analytics Pane - Native Time Series Forecast
- **Version Control**: GitHub
- **Documentation**: Markdown

## Methods
1. **Data Cleaning**: Removed 23 null Sales records, converted Order Date to Date type, eliminated duplicate Order IDs, standardized Region/Segment names using Power Query
2. **Data Modeling**: Created DAX measures - `Total Sales = SUM(Sales)`, `Total Profit = SUM(Profit)`, `Profit Margin = DIVIDE([Total Profit], [Total Sales])`
3. **Visualization**: Built 12+ visuals including KPI Cards, Line Charts, Donut Charts, Filled Maps, Bar Charts with slicers for Year, Region, Segment, Category
4. **Forecasting**: Applied Power BI's built-in forecasting model on Sales measure with Seasonality set to 12, Confidence Interval 95%, Forecast Length 6 months

## Key Insights
1. **Sales Trend**: Revenue grew from ~13K in 2014 to ~101K in 2017, showing consistent YoY growth
2. **Top Segment**: Technology segment contributes highest sales across all 4 years
3. **Regional Leader**: West US region dominates sales, followed by East region on the filled map
4. **Discount Impact**: 20% discount level drives maximum sales volume without major profit loss
5. **Seasonality**: Q4 shows recurring sales spikes every year indicating holiday demand
6. **Forecast**: Model predicts continued upward trend for next 6 months with upper/lower confidence bands

## Dashboard/Model/Output
![Dashboard Screenshot](dashboard_screenshot.png)

**Dashboard Components:**
- **Top Row**: KPI Cards - Total Sales, Total Profit, Profit Margin, Total Orders + Year Slicer
- **Middle**: Predictive Sales Forecast line chart with 6-month projection + Sales by Segment Donut
- **Bottom**: Regional Sales Filled Map + Sales by Discount Bar Chart + Category Performance

**Files:**
- `Sales_Forecast_Dashboard.pbix` - Main Power BI file
- `dashboard_screenshot.png` - Dashboard preview

## How to Run this project?
### Prerequisites:
1. Download [Power BI Desktop](https://powerbi.microsoft.com/desktop/) - Free

### Steps:
1. Clone this repository:
   ```bash
   git clone https://github.com/ladtanvi12-lab/predictive-sales-forecast-powerbi.git
