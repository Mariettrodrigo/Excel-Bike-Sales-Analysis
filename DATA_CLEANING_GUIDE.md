# Data Cleaning Documentation

## Overview
This document outlines the data cleaning process performed on the bike sales dataset to prepare it for analysis through pivot tables and visualization.

## Raw Data Issues Identified

### 1. Inconsistent Gender Coding
- **Issue**: Gender was coded as "M" and "F" which is not immediately clear
- **Solution**: Replaced with "Male" and "Female" for clarity

### 2. Marital Status Abbreviations
- **Issue**: Marital status used "M" for Married and "S" for Single
- **Solution**: Expanded abbreviations to full words "Married" and "Single"

### 3. Missing Age Brackets
- **Issue**: No age grouping for easier analysis and visualization
- **Solution**: Added "Age Bracket" column with categories:
  - Young Adult: 25-40 years
  - Middle Age: 41-54 years
  - Old: 55+ years

## Data Cleaning Steps

### Step 1: Replace Gender Abbreviations
```
Find: M (in Gender column)
Replace: Male

Find: F (in Gender column)
Replace: Female
```

### Step 2: Expand Marital Status
```
Find: M (in Marital Status column)
Replace: Married

Find: S (in Marital Status column)
Replace: Single
```

### Step 3: Create Age Bracket Column
Added a new column "Age Bracket" with the following logic:
- IF Age < 41, THEN "Young Adult"
- IF Age >= 41 AND Age <= 54, THEN "Middle Age"
- IF Age > 54, THEN "Old"

Excel Formula: `=IF(L2<41,"Young Adult",IF(L2<=54,"Middle Age","Old"))`

### Step 4: Data Validation
- Verified no duplicate IDs
- Checked for null values (none found)
- Confirmed all numerical fields contain valid numbers
- Validated categorical fields contain expected values
- Ensured consistency in date formats and text fields

## Data Quality Checks

### Completeness
- ✓ All rows have values in all columns
- ✓ No missing or null values identified
- ✓ 100 complete customer records

### Consistency
- ✓ Gender values standardized to "Male" and "Female"
- ✓ Marital status values standardized to "Married" and "Single"
- ✓ Region names consistent across dataset
- ✓ Commute distance categories uniform

### Accuracy
- ✓ Income values within reasonable range ($30,000 - $100,000)
- ✓ Age values realistic (28-61 years)
- ✓ Children count reasonable (0-5)
- ✓ Car ownership aligned with income levels

## Field Descriptions

| Field Name | Type | Description | Valid Values |
|------------|------|-------------|--------------|
| ID | Number | Unique customer identifier | Integer |
| Marital Status | Text | Customer's marital status | Married, Single |
| Gender | Text | Customer's gender | Male, Female |
| Income | Number | Annual income in dollars | 30000-100000 |
| Children | Number | Number of children | 0-5 |
| Education | Text | Highest education level | Partial High School, High School, Partial College, Bachelors, Graduate Degree |
| Occupation | Text | Customer's occupation type | Manual, Skilled Manual, Clerical, Professional, Management |
| Home Owner | Text | Home ownership status | Yes, No |
| Cars | Number | Number of cars owned | 0-4 |
| Commute Distance | Text | Distance to work | 0-1 Miles, 1-2 Miles, 2-5 Miles, 5-10 Miles, 10+ Miles |
| Region | Text | Geographic region | Europe, North America, Pacific |
| Age | Number | Customer's age in years | 28-61 |
| Age Bracket | Text | Age category | Young Adult, Middle Age, Old |
| Purchased Bike | Text | Whether customer purchased a bike | Yes, No |

## Data Export Format

The cleaned data is saved in CSV format with:
- UTF-8 encoding
- Comma delimiters
- Header row included
- No special characters requiring escaping

## Next Steps

After data cleaning, the dataset is ready for:
1. Pivot table creation for analysis
2. Dashboard visualization
3. Insights generation
