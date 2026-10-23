# Agricultural-crop-yield-analysis
An agricultural data analytics capstone project using Microsoft Excel and Power BI to analyze crop yield patterns, explore environmental and farming-related factors, and present actionable insights through interactive dashboards.
# Analysis of Factors Influencing Agricultural Crop Yield and Productivity

## Project Overview

This project analyzes agricultural crop yield data to identify patterns and relationships between crop productivity and selected environmental and farming-related factors. The analysis focuses on rainfall, temperature, soil type, crop type, fertilizer use, irrigation, weather conditions, and days to harvest.

Microsoft Excel was used for data cleaning, exploratory data analysis (EDA), descriptive statistics, correlation analysis, and PivotTable analysis. Microsoft Power BI was used to develop an interactive, three-page dashboard presenting the results, key insights, and recommendations.

The project demonstrates how data analytics can support agricultural decision-making by identifying patterns in crop yield and highlighting areas that may warrant further investigation.

## Problem Statement

Agricultural productivity is influenced by multiple environmental and farming-related factors. Understanding how these factors relate to crop yield can help stakeholders identify patterns, evaluate farming practices, and make more informed decisions.

This project examines a crop-yield dataset to determine which variables show the strongest observed relationships with yield and which categories display similar average productivity. The analysis also considers the limitations of the available data when interpreting the findings.

## Project Objectives

The objectives of this project are to:

1. Clean and validate the agricultural crop-yield dataset.
2. Examine the distribution and descriptive statistics of the numerical variables.
3. Compare average yield across crops, regions, and soil types.
4. Assess differences in average yield between records with and without fertilizer and irrigation use.
5. Investigate the relationships between yield and rainfall, temperature, weather conditions, and days to harvest.
6. Develop an interactive Power BI dashboard to communicate the findings.
7. Provide evidence-based recommendations while acknowledging the limitations of the analysis.

## Dataset Description

**Dataset:** Agriculture Crop Yield  
**Author:** Samuel Oti Attakorah  
**Source:** [Kaggle — Agriculture Crop Yield Dataset](https://www.kaggle.com/datasets/samuelotiattakorah/agriculture-crop-yield/data)

The original dataset contained 1,000,000 records and 10 columns. It includes categorical variables describing agricultural conditions and numerical variables measuring environmental conditions, harvest timing, and crop yield.

### Variables used

| Variable | Description |
|---|---|
| Region | Agricultural region: East, North, South, or West |
| Soil_Type | Soil category |
| Crop | Crop type |
| Rainfall_mm | Rainfall measurement in millimeters |
| Temperature_Celsius | Temperature in degrees Celsius |
| Fertilizer_Used | Indicates whether fertilizer use was recorded |
| Irrigation_Used | Indicates whether irrigation use was recorded |
| Weather_Condition | Recorded weather condition |
| Days_to_Harvest | Number of days to harvest |
| Yield_tons_per_hectare | Crop yield in tons per hectare; the primary outcome variable |

The dataset does not contain a year variable for individual observations, so the analysis does not assess year-over-year changes.

## Tools and Technologies

- **Microsoft Excel:** Data cleaning, data validation, descriptive statistics, correlation analysis, calculated fields, PivotTables, and exploratory analysis.
- **Microsoft Power BI Desktop:** Interactive dashboards, KPI cards, charts, slicers, and presentation of analytical findings.
- **GitHub:** Project documentation, portfolio organization, and sharing of project deliverables.

## Methodology

### 1. Data inspection

The original dataset was inspected in Excel to understand its structure, column names, data types, categorical values, and numerical ranges.

The initial inspection identified 1,000,000 records across 10 columns, with no missing values or duplicate records reported.

### 2. Data cleaning and validation

A separate cleaned worksheet was created to preserve the original dataset.

The cleaning process included:

- Checking for missing values.
- Checking for duplicate records.
- Reviewing numerical ranges and identifying invalid yield values.
- Filtering the yield column to identify negative values.
- Removing 231 records with negative crop yields, which were treated as invalid for this analysis.
- Retaining zero-yield observations because zero is a valid numerical value.
- Rechecking the cleaned dataset after removal.

The final analytical dataset contained **999,769 records**, with no missing values, no duplicate records, and no remaining negative yield values.

### 3. Exploratory data analysis

Excel was used to calculate descriptive statistics and compare average yield across different categories.

The analysis included:

- Average yield by crop.
- Average yield by region.
- Average yield by soil type.
- Average yield by fertilizer use.
- Average yield by irrigation use.
- Average yield by weather condition.
- Average yield across rainfall bands.
- Average yield across temperature bands.
- Average yield across days-to-harvest groups.
- Correlation analysis between yield and selected numerical variables.

### 4. Power BI visualization

The cleaned dataset was imported into Power BI Desktop to create a three-page interactive report.

**Page 1 — Executive Dashboard**
- Total records analyzed.
- Overall average crop yield.
- Average yield comparisons by fertilizer and irrigation use.
- Yield comparisons across regions and crops.
- Slicers for selected categorical variables.

**Page 2 — Environmental & Production Analysis**
- Average yield by rainfall band.
- Average yield by temperature band.
- Average yield by soil type.
- Average yield by weather condition.
- Average yield by crop.
- Average yield by days-to-harvest group.
- Region, Crop, and Soil Type slicers.

**Page 3 — Key Insights & Recommendations**
- Key findings on rainfall, fertilizer, and irrigation.
- Recommended actions based on the observed patterns.
- Limitations to consider when interpreting the results.

## Key Findings

### 1. Rainfall showed the strongest positive correlation with yield

The correlation between rainfall and crop yield was **0.7645**, indicating a strong positive linear association in the cleaned dataset.

Average yield increased across the rainfall bands, from approximately **2.66 tons per hectare** in the 100–199 mm band to approximately **6.65 tons per hectare** in the 900–1000 mm band.

This pattern suggests that rainfall is an important variable to investigate when examining crop yield in this dataset. It does not establish that rainfall alone causes higher yield.

### 2. Fertilizer use was associated with higher average yield

| Fertilizer use recorded | Average yield (tons/ha) |
|---|---:|
| False | 3.90 |
| True | 5.40 |

Records where fertilizer use was recorded as True had a higher average yield than records where it was recorded as False.

This is an observed association, not proof of a causal effect.

### 3. Irrigation use was associated with higher average yield

| Irrigation use recorded | Average yield (tons/ha) |
|---|---:|
| False | 4.05 |
| True | 5.25 |

Records where irrigation use was recorded as True had a higher average yield than records where it was recorded as False. Further analysis would be required to determine how irrigation interacts with other factors.

### 4. Temperature showed a weak positive relationship with yield

The correlation between temperature and yield was **0.0852**, indicating a weak positive linear relationship.

Although average yield increased across the temperature bands, the correlation suggests that temperature alone had a weak linear association with yield in the analyzed data.

### 5. Days to harvest showed essentially no linear relationship with yield

The correlation between days to harvest and yield was approximately **-0.0026**, indicating virtually no linear relationship in the dataset.

Average yields were also very similar across the days-to-harvest groups.

### 6. Average yield was similar across crop, region, soil, and weather categories

The average yields across the six crop categories, four regions, six soil types, and three weather conditions were closely clustered.

This suggests that these categories, when examined individually through average yield, showed relatively little variation in this dataset. Their possible interactions with other variables warrant further investigation.

## Recommendations

Based on the observed patterns, the following actions are recommended for further investigation:

1. **Monitor rainfall conditions:** Investigate rainfall patterns alongside crop requirements, drainage, and water availability to support agricultural planning.
2. **Evaluate fertilizer practices:** Examine fertilizer type, application rates, timing, and crop-specific requirements before drawing conclusions about its effectiveness.
3. **Assess irrigation practices:** Investigate irrigation access, water management, and interactions between irrigation and rainfall.
4. **Examine multiple variables together:** Explore interactions among environmental conditions, farming practices, soil types, and crop types rather than relying on individual averages.
5. **Improve future data collection:** Include farm-level information, locations, crop varieties, management practices, and observation years to enable more detailed comparisons and stronger analysis.

These recommendations are intended to guide further investigation rather than prescribe interventions based on association alone.

## Limitations

- The analysis identifies associations and patterns; it does not establish causation.
- The dataset does not provide a year variable for individual records, preventing year-over-year analysis.
- Negative yield records were excluded as invalid, reducing the dataset from 1,000,000 to 999,769 records.
- The analysis relies on the variables available in the dataset. Other factors that may influence agricultural productivity are not necessarily captured.
- Similar average yields across categories do not rule out differences within subgroups or interactions between variables.
- Findings should be validated with relevant local agricultural evidence before being applied to specific farms or regions.

## Project Deliverables

The project deliverables include:

1. Original agricultural crop-yield dataset.
2. Cleaned Excel dataset.
3. Excel exploratory analysis and descriptive statistics.
4. Excel PivotTables and supporting charts.
5. Three-page interactive Power BI dashboard.
6. Key findings, recommendations, and limitations.
7. GitHub project documentation and portfolio materials.

## Conclusion

This project used Microsoft Excel and Power BI to examine agricultural crop-yield data and communicate the results through an interactive dashboard.

Rainfall showed the strongest positive linear association with yield among the numerical variables examined, while fertilizer and irrigation use were associated with higher average yields. Temperature showed a weak positive relationship, and days to harvest showed virtually no linear relationship. Average yields were also similar across crop, region, soil, and weather categories when examined individually.

Overall, the analysis demonstrates how data cleaning, exploratory analysis, correlation, and visualization can help identify useful patterns in agricultural data while emphasizing the importance of careful interpretation and further validation.

---

**Project title:** Analysis of Factors Influencing Agricultural Crop Yield and Productivity  
**Tools:** Microsoft Excel | Microsoft Power BI Desktop  
**Dataset source:** Kaggle  
**Author:** Kingsley Chimezie Nwobodo  
**Project type:** Data Analytics Capstone Project
