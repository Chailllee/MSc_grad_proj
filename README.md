# Evaluating the Impact of Ultra Low Emission Zone Policies on Air Quality and Public Transportation Choices in Central London

## Overview

This repository contains the research and analysis conducted for the MSc dissertation titled *Evaluating the Impact of Ultra Low Emission Zone Policies on Air Quality and Public Transportation Choices in Central London* by Xiaoyi. The study assesses the effectiveness of ULEZ in reducing air pollution and influencing public transportation usage.

## Abstract

This study evaluates the impact of the Ultra-Low Emission Zone (ULEZ) policy on air quality and public transportation in Central London from 2019 to 2024. Using data on Nitric Oxide (NO), Nitrogen Dioxide (NO2), PM2.5, and PM10 levels, along with traffic flow and public transportation statistics, the research employs spatial interpolation and Kriging techniques to analyze changes in air quality. The findings highlight significant improvements in air quality, particularly reductions in NO and NO2 levels, providing insights for future urban policy planning.

## Methodology

- **Data Sources:** Air pollution levels, traffic flow, and public transport statistics from government and open datasets.
- **Data Processing:** Missing value interpolation and Kriging-based spatial interpolation.
![Data processing flowchart](others\Figure 3 Data processing flowchart.png)
- **Analysis Techniques:** Exploratory Data Analysis (EDA), time-series analysis, and regression modeling.

## Key Findings

- ULEZ implementation led to notable reductions in NO and NO2 levels, particularly in high-traffic areas like the City of London, Camden, and Kensington.

<p align="center">
    <img src="others/Figure%203%20Data%20processing%20flowchart.png" alt="Data processing flowchart" width="480"/>
</p>

- Public transportation usage saw an increase, suggesting a behavioral shift due to the policy.
- Kriging-based spatial interpolation effectively estimated air quality improvements in targeted zones.
-
-

## Repository Structure

```
├── 1Interpolation/      # Code and data related to interpolation techniques
├── 2Kriging/            # Kriging-based spatial interpolation files
├── 3Method/             # Methods and scripts for data analysis
│   ├── 3-1EDA/          # Exploratory Data Analysis
│   ├── 3-2Correlation/  # Correlation analysis
│   └── 3-3Diff/         # Difference-based analysis
├── Data/                # Raw datasets used in the project
│   ├── AirQuality/      # Air quality data
│   ├── dfl_traffic_count/ # Traffic count data
│   ├── london_boundaries/ # Geographic boundaries of London
│   ├── meteoStat/       # Meteorological data
│   ├── tfl_crowding_data/ # Transport for London crowding data
│   └── tfl_geo_data/    # Geographic data from Transport for London
├── Data_output/         # Processed data outputs and intermediate results
├── others/              # Miscellaneous files and scripts (not directly related to the dissertation; can be ignored)
├── Evaluating the Impact of Ultra Low Emission Zone Policies on Air Quality and Public Transportation Choices in Central London.pdf  
                         # MSc Dissertation document
├── README.md            # Project documentation
```
## Citation

If you find this work useful, please cite:
**Chen, Xiaoyi (2024). Evaluating the Impact of Ultra Low Emission Zone Policies on Air Quality and Public Transportation Choices in Central London. MSc Dissertation, UCL.**

## Contact

For any questions or collaborations, feel free to reach out via GitHub issues or email.



## Improvements and Future Work

Based on feedback from the dissertation markers, several areas for improvement have been identified:

1. **Research Framing and Design**:  
   - The introduction is concise, but could have better signposted the structure of the paper, chapter by chapter, and provided a summary of key results and their implications.  
   - A broader review of econometric literature related to driving restrictions and their effects on air quality would have strengthened the literature review. In particular, methods such as difference-in-differences and regression discontinuity, often used in policy evaluation, would have provided greater analytical depth.

2. **Analysis and Critical Reflection**:  
   - The time series analysis took on a descriptive nature rather than analytical. A regression discontinuity approach would have allowed for more precise measurements of policy effects.  
   - The "difference between periods" section could benefit from a Difference-in-Differences approach, which would generate more statistically significant insights into the impact of ULEZ.
   - The correlation analysis was too broad and included peripheral data. Narrowing the focus would strengthen the analysis.
   - Regression results were not presented in the standard way, lacking p-values, standard errors, and R-squared values. Reorganizing these results in a table would provide clearer insights.

3. **Visualization**:  
   - Some figures, such as **Figure 4.1.1**, could be reworked to be more information-dense, improving comparison across boroughs.
   - **Figure 4.2.1** was found to be too crowded and large, making it difficult to extract meaningful insights.

These insights will inform future work and revisions to the analysis and presentation.

