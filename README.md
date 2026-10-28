# Agricultural Crop Yield Analysis

## Project Overview

This capstone project analyzes agricultural crop yield data to explore how rainfall, temperature, soil type, weather conditions, fertilizer use, irrigation, and harvest timing relate to crop productivity.

Using Microsoft Excel and Power BI, the project demonstrates data cleaning, exploratory data analysis, statistical comparison, data visualization, and the communication of actionable insights.

## Project Objectives

- Examine average crop yield across crop types, regions, and soil types.
- Explore the relationship between rainfall, temperature, and crop yield.
- Compare average yield between records with and without fertilizer use and irrigation.
- Investigate yield patterns across weather conditions and harvest-time groups.
- Present key findings, recommendations, and limitations through interactive Power BI dashboards.

## Dataset

**Source:** [Agriculture Crop Yield — Kaggle](https://www.kaggle.com/datasets/samuelotiattakorah/agriculture-crop-yield/data)

The dataset contains agricultural observations covering regional, environmental, and farming-related variables, including rainfall, temperature, crop type, soil type, fertilizer use, irrigation use, weather condition, days to harvest, and yield in tons per hectare.

The cleaned analytical dataset contains **999,769 records** after 231 records with negative yield values were excluded during data validation.

## Tools Used

- **Microsoft Excel:** Data inspection, cleaning, descriptive statistics, PivotTables, and exploratory analysis.
- **Microsoft Power BI:** Interactive dashboards, KPI cards, charts, slicers, and insight reporting.
- **GitHub:** Project documentation, version control, and portfolio presentation.

## Methodology

1. Inspected the source data and reviewed variable types and category values.
2. Checked for missing values and duplicate records.
3. Investigated negative yield values and excluded 231 such records from the cleaned analytical dataset.
4. Calculated descriptive statistics and compared average yield across relevant categories.
5. Examined correlations and yield patterns across rainfall, temperature, and days-to-harvest groups.
6. Built Power BI dashboards to present the findings and recommendations.
7. Documented analytical insights, limitations, and areas for further investigation.

## Key Findings

- **Rainfall:** The strongest observed linear association with yield was positive, with a correlation coefficient of approximately **0.7645**. Average yield increased across the rainfall bands in the dataset.
- **Fertilizer use:** Records marked as using fertilizer had an average yield of approximately **5.40 tons/ha**, compared with **3.90 tons/ha** for records marked as not using fertilizer.
- **Irrigation:** Records marked as using irrigation had an average yield of approximately **5.25 tons/ha**, compared with **4.05 tons/ha** for records marked as not using irrigation.
- **Temperature:** The observed linear relationship with yield was weakly positive, with a correlation coefficient of approximately **0.0852**.
- **Days to harvest:** The correlation with yield was approximately **-0.0026**, indicating virtually no linear relationship in this dataset.
- **Crop, region, soil type, and weather:** Average yields were relatively similar across their respective categories.

These findings describe associations and patterns in the dataset; they do not establish that any individual factor causes higher crop yield.

## Power BI Dashboard Screenshots

### 1. Executive Dashboard

![Executive Dashboard](Images/Executive-dashboard.png%20%E2%80%94%20Page%201.png)

### 2. Environmental & Production Analysis

![Environmental & Production Analysis](Images/Environmental-analysis.png%20%E2%80%94%20Page%202.png)

### 3. Key Insights & Recommendations

![Key Insights & Recommendations](Images/Insights-recommendations.png%20%E2%80%94%20Page%203.png)


## Recommendations

- Investigate rainfall patterns when planning agricultural activities, while considering crop requirements and local conditions.
- Evaluate fertilizer practices, application rates, and soil conditions before making farm-level recommendations.
- Assess irrigation access and water-management practices.
- Explore interactions among environmental and farming factors rather than relying on one variable alone.
- Validate these findings with additional local or farm-level data before applying them to specific agricultural settings.

## Limitations

- The analysis identifies associations, not causal effects.
- The dataset does not provide a year-by-year comparison.
- Negative yield records were excluded as part of data validation.
- The observed relationships may not generalize to every crop, farm, or region.
- Additional context and domain validation are needed before making operational farming decisions.

## Project Deliverables

- Cleaned agricultural data and Excel analysis summary.
- Exploratory analysis and comparative statistics.
- Three-page Power BI dashboard.
- Key findings, recommendations, and limitations.
- Project documentation hosted on GitHub.

## Conclusion

This project demonstrates how Excel and Power BI can be used to prepare agricultural data, explore factors associated with crop yield, and communicate analytical findings through clear visualizations. The results highlight rainfall as the strongest observed linear correlate of yield in this dataset, while also showing notable differences between records marked for fertilizer and irrigation use.

The project provides a foundation for further agricultural analysis and evidence-informed investigation.
