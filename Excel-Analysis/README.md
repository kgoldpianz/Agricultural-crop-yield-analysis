# Excel Data Analysis

## Overview

This folder contains the Excel-based data preparation and exploratory analysis for the Agricultural Crop Yield Analysis capstone project.

Microsoft Excel was used to inspect the dataset, identify invalid yield records, clean the data, summarize key variables, and compare average crop yields across environmental and agricultural conditions.

## Dataset

- **Source:** [Agriculture Crop Yield Dataset — Kaggle](https://www.kaggle.com/datasets/samuelotiattakorah/agriculture-crop-yield/data)
- **Original records:** 1,000,000
- **Records removed:** 231 records with negative yield values
- **Final cleaned records:** 999,769

The dataset includes region, soil type, crop, rainfall, temperature, fertilizer use, irrigation use, weather condition, days to harvest, and yield in tons per hectare.

## Data Cleaning

The following steps were performed in Excel:

1. Inspected the original dataset and checked the available columns.
2. Reviewed the data for missing values and duplicate records.
3. Identified 231 records with negative crop-yield values.
4. Removed those invalid negative-yield records while retaining zero-yield records.
5. Preserved the original dataset and maintained a backup of the cleaned data.
6. Checked the cleaned dataset to confirm the final record count.

The cleaned dataset contained 999,769 records. No missing values or duplicate records were identified in the final cleaned data during the checks performed.

## Exploratory Data Analysis

Excel was used to calculate descriptive statistics, create summary tables and PivotTables, compare average yields across categories, and examine relationships between yield and selected numerical variables.

The analysis covered:

- Average yield by crop, region, and soil type
- Yield differences associated with fertilizer and irrigation use
- Yield comparisons across weather conditions
- Relationships between rainfall, temperature, days to harvest, and crop yield
- Average yield across rainfall, temperature, and harvest-time bands

## Key Findings

- **Overall average yield:** Approximately 4.65 tons per hectare.
- **Rainfall:** The correlation between rainfall and yield was approximately 0.7645, indicating a strong positive linear association in this dataset.
- **Fertilizer use:** Records marked as using fertilizer had an average yield of approximately 5.40 tons per hectare, compared with 3.90 for records without fertilizer use.
- **Irrigation:** Records marked as using irrigation had an average yield of approximately 5.25 tons per hectare, compared with 4.05 for records without irrigation.
- **Temperature:** The correlation with yield was approximately 0.0852, indicating a weak positive linear association.
- **Days to harvest:** The correlation with yield was approximately -0.0026, indicating virtually no linear relationship.
- **Crop, region, soil, and weather categories:** Average yields were relatively similar across these groups in the dataset.

These results describe observed associations and group averages; they do not establish that any single factor caused a change in yield.

## Tools Used

- Microsoft Excel
- Excel Tables
- Formulas and descriptive statistics
- PivotTables
- Correlation analysis

## Project Deliverables

This folder contains the Excel analysis summary workbook. The original large dataset was retained locally because of its size; the dataset source is linked above.

The Power BI dashboard screenshots and project overview are available in the main repository README.

## Conclusion

The Excel analysis provided a structured foundation for the capstone project by cleaning the data, summarizing important variables, and identifying relationships for further exploration in Power BI.
