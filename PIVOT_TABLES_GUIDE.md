# Pivot Table and Analysis Guide

## Overview
This guide provides instructions for creating pivot tables in Excel to analyze the bike sales data.

## Recommended Pivot Tables

### Pivot Table 1: Bike Sales by Demographics

**Purpose**: Analyze purchase rates across different demographic segments

**Setup Instructions**:
1. Select the entire cleaned data table
2. Insert → PivotTable
3. Place in new worksheet, name it "Demographics Analysis"

**Configuration**:
- **Rows**: Gender, Marital Status
- **Columns**: Purchased Bike
- **Values**: Count of ID
- **Filters**: Region, Age Bracket

**Additional Calculation**:
- Add calculated field for purchase rate: `=Count of Yes / (Count of Yes + Count of No)`

### Pivot Table 2: Income Analysis

**Purpose**: Understand the relationship between income levels and bike purchases

**Setup Instructions**:
1. Insert → PivotTable from cleaned data
2. Place in new worksheet, name it "Income Analysis"

**Configuration**:
- **Rows**: Purchased Bike
- **Values**: 
  - Average of Income
  - Min of Income
  - Max of Income
  - Count of ID
- **Filters**: Gender, Marital Status, Age Bracket

**Additional Analysis**:
- Group income into brackets:
  - Low Income: $30,000-$50,000
  - Middle Income: $51,000-$70,000
  - High Income: $71,000+

### Pivot Table 3: Commute Distance vs. Bike Purchase

**Purpose**: Analyze how commute distance affects bike purchase decisions

**Setup Instructions**:
1. Insert → PivotTable from cleaned data
2. Place in new worksheet, name it "Commute Analysis"

**Configuration**:
- **Rows**: Commute Distance
- **Columns**: Purchased Bike
- **Values**: Count of ID
- **Filters**: Region, Age Bracket

**Sort**: Order commute distance categories logically (0-1 Miles → 10+ Miles)

### Pivot Table 4: Regional Analysis

**Purpose**: Compare bike sales performance across different regions

**Setup Instructions**:
1. Insert → PivotTable from cleaned data
2. Place in new worksheet, name it "Regional Analysis"

**Configuration**:
- **Rows**: Region
- **Columns**: Purchased Bike
- **Values**: 
  - Count of ID
  - Average of Income
  - Average of Age
- **Filters**: Gender, Marital Status

### Pivot Table 5: Age and Education Impact

**Purpose**: Analyze how age brackets and education levels affect purchases

**Setup Instructions**:
1. Insert → PivotTable from cleaned data
2. Place in new worksheet, name it "Age-Education Analysis"

**Configuration**:
- **Rows**: Age Bracket, Education
- **Columns**: Purchased Bike
- **Values**: Count of ID, Average of Income
- **Filters**: Gender, Region

### Pivot Table 6: Occupation and Car Ownership

**Purpose**: Understand the relationship between occupation, car ownership, and bike purchases

**Setup Instructions**:
1. Insert → PivotTable from cleaned data
2. Place in new worksheet, name it "Occupation Analysis"

**Configuration**:
- **Rows**: Occupation, Cars
- **Columns**: Purchased Bike
- **Values**: Count of ID
- **Filters**: Region, Income (grouped)

## Pivot Table Formatting Best Practices

### Number Formatting
- **Income**: Currency format with $ symbol, no decimals
- **Counts**: Number format with comma separator
- **Percentages**: Percentage format with 1 decimal place

### Styling
- Apply a professional PivotTable style (Design tab)
- Use banded rows for better readability
- Bold column headers
- Apply conditional formatting to highlight key insights

### Slicers
Add slicers for easy filtering:
1. Click on pivot table
2. Insert → Slicer
3. Add slicers for:
   - Region
   - Age Bracket
   - Marital Status
   - Gender

Format slicers to match dashboard theme.

## Key Metrics to Calculate

### 1. Purchase Conversion Rate
```
Formula: =COUNTIF(PurchasedBike,"Yes")/COUNTA(PurchasedBike)
```

### 2. Average Customer Value (by segment)
```
Use average income of customers who purchased bikes
```

### 3. Regional Market Penetration
```
Calculate percentage of customers who purchased in each region
```

### 4. Demographic Conversion Rates
```
Calculate purchase rate for each demographic segment
Compare to overall average
```

## Analysis Questions to Answer

1. **Which demographic group has the highest bike purchase rate?**
   - Gender comparison
   - Marital status comparison
   - Age bracket comparison

2. **What is the optimal income range for bike customers?**
   - Average income of buyers vs. non-buyers
   - Income distribution of successful sales

3. **How does commute distance impact purchase decisions?**
   - Purchase rates by distance category
   - Identify sweet spot for bike commuting

4. **Which region shows the most promise for marketing?**
   - Regional purchase rates
   - Regional income levels
   - Regional demographic profiles

5. **What is the typical buyer profile?**
   - Most common characteristics of bike buyers
   - Differences from non-buyers

## Tips for Effective Pivot Table Analysis

1. **Start with broad categories, then drill down**
2. **Use filters to isolate specific segments**
3. **Compare percentages, not just raw counts**
4. **Look for unexpected patterns or anomalies**
5. **Create multiple views of the same data**
6. **Refresh pivot tables after any data changes**
7. **Document insights as you discover them**

## Refreshing Pivot Tables

When source data is updated:
1. Right-click on pivot table
2. Select "Refresh"
3. Or use "Refresh All" to update all pivot tables

Keyboard shortcut: **Alt + F5**
