# 📊 Power BI Project: Customer Returns Analysis

## 🧭 Executive Summary
This Power BI dashboard provides a comprehensive analysis of customer return behavior across products, categories, subcategories, and geographic territories. It helps stakeholders identify patterns, reduce return rates, and improve product and regional strategies.

## 🎯 Business Objectives

- Detect high-return products and investigate root causes
- Analyze category and subcategory trends to uncover systemic issues
- Compare return rates across territories to inform regional decisions
- Understand customer return reasons to improve satisfaction
- Monitor return trends over time to evaluate business impact

## 📁 Data Model Overview

The dashboard integrates multiple structured tables:

| Table Name     | Description |
|----------------|-------------|
| Returns        | Transaction-level data with customer ID, product ID, return date, reason, and territory |
| Products       | Product metadata including name, category, subcategory, and price |
| Categories     | Hierarchical mapping of categories and subcategories |
| Territories    | Regional mapping of customer locations |
| Calendar       | Date table for time-based analysis (month, quarter, year)

### 🔗 Relationships

- Returns[ProductID] → Products[ProductID]
- Products[CategoryID] → Categories[CategoryID]
- Returns[TerritoryID] → Territories[TerritoryID]
- Returns[ReturnDate] → Calendar[Date]

## 📊 Dashboard Features

### 1. Return Rate Analysis
- Highlights top returned products by volume and percentage
- Normalizes return rates by sales volume (if available)

### 2. Category & Subcategory Breakdown
- Treemaps and bar charts showing return distribution
- Drill-through to subcategory and individual product levels

### 3. Territory Comparison
- Map visuals showing regional return rates
- Filters for country, state, and city-level insights

### 4. Time Series Trends
- Monthly and quarterly return trends
- Year-over-year comparisons

### 5. Return Reason Analysis
- Pie charts and bar graphs of return reasons
- Cross-filtering with product and territory data

### 6. Interactive Filters
- Slicers for:
  - Date range
  - Product category/subcategory
  - Territory
  - Return reason

## 🧠 Measures & Calculations

All key metrics and KPIs in the dashboard are powered by **DAX measures**, including calculations for return rates, top returned products, and time-based trends. These measures ensure dynamic filtering and accurate aggregation across visuals.

## 🛠️ Setup Instructions

1. Open the `.pbix` file in Power BI Desktop
2. Connect to your data sources or refresh sample data
3. Review relationships in the data model
4. Customize visuals to match your business needs
5. Publish to Power BI Service for sharing and scheduled refresh


## 📬 Contact & Support

For questions, feedback, or collaboration, contact:

**Mohammed Ashraf**  
📧 moashraf9877570@gmail.com  
🌍 Based in Al Jizah, Egypt
