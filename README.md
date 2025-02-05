# Evaluating the Impact of Ultra Low Emission Zone Policies on Air Quality and Public Transportation Choices in Central London

## Overview

This repository contains the research and analysis conducted for the MSc dissertation titled *Evaluating the Impact of Ultra Low Emission Zone Policies on Air Quality and Public Transportation Choices in Central London* by Xiaoyi. The study assesses the effectiveness of ULEZ in reducing air pollution and influencing public transportation usage.

<p align="center">
   <img src="others\Map of the Low Emission Zone (LEZ) and ULEZ boundaries.png" alt="Map of the Low Emission Zone (LEZ) and ULEZ boundaries" width="550"/>
</p>
<p align="center">
   <em>Fig.1: Map of the Low Emission Zone (LEZ) and ULEZ boundaries.</em>
</p>

## Abstract

This study evaluates the impact of the Ultra-Low Emission Zone (ULEZ) policy on air quality and public transportation in Central London from 2019 to 2024. Using data on Nitric Oxide (NO), Nitrogen Dioxide (NO2), PM2.5, and PM10 levels, along with traffic flow and public transportation statistics, the research employs spatial interpolation and Kriging techniques to analyze changes in air quality. The findings highlight significant improvements in air quality, particularly reductions in NO and NO2 levels, providing insights for future urban policy planning.

## Methodology

- **Data Sources:** Air pollution levels, traffic flow, and public transport statistics from government and open datasets.
- **Data Processing:** Missing value interpolation and Kriging-based spatial interpolation.

<p align="center">
   <img src="others/Figure%203%20Data%20processing%20flowchart.png" alt="Data processing flowchart" width="480"/>
</p>
<p align="center">
   <em>Fig.2: This flowchart illustrates the data processing steps, including data collection, missing value interpolation, and Kriging-based spatial interpolation, used to analyze the impact of ULEZ policies in Central London.</em>
</p>

- **Analysis Techniques:** Exploratory Data Analysis (EDA), time-series analysis, and regression modeling.

## Key Findings


1. **Significant Reduction in Air Pollution Levels**
   - The **Ultra-Low Emission Zone (ULEZ)** policy led to **notable decreases in Nitric Oxide (NO) and Nitrogen Dioxide (NO2) levels**, especially in the later expansion stages (2021 & 2023).

<p align="center">
   <img src="others\time trend NO.png" alt="Time trend of Nitric Oxide (NO) levels" width="45%" style="display: inline-block;"/>
   <img src="others\time trend NO2.png" alt="Time trend of Nitrogen Dioxide (NO2) levels" width="45%" style="display: inline-block;"/>
</p>
<p align="center">
   <em>Fig.3: Time trends of Nitric Oxide (NO) and Nitrogen Dioxide (NO2) levels from 2019 to 2024, showing the impact of ULEZ policy implementations.</em>
</p>

   - **Westminster, Camden, and Kensington & Chelsea** saw the most substantial improvements in air quality.
   - **PM2.5 and PM10 levels** showed moderate improvement, but further measures may be needed for sustained reductions.

2. **Shift in Public Transport Usage**
   - ULEZ **encouraged higher public transport usage**, with increased ridership in underground stations within the policy zones.
   - Reduction in private vehicle use contributed to overall improvements in **air quality and reduced traffic congestion**.

3. **Effectiveness of Spatial Interpolation (Kriging)**
   - **Kriging interpolation** was used to estimate air quality changes across the city, accounting for sensor data and meteorological factors (wind speed, wind direction).
   - This method provided more accurate assessments compared to simple averaging techniques.

4. **Impact Varied by Implementation Stage**
   - **2019 ULEZ Central Zone Launch**: Initial improvements in NO2 and PM levels, but mixed results due to limited coverage.
   - **2021 Inner Expansion**: Reinforced earlier improvements, with significant NO2 reductions in Southwark and Kensington & Chelsea.
   - **2023 Outer Expansion**: Largest and most consistent decrease in NO and NO2 levels across all regions.

5. **Limitations and Future Considerations**
   - Some **regions, like the City of London and Camden, showed smaller improvements**, suggesting baseline pollution levels or external factors may have influenced outcomes.
   - **ULEZ policies had a stronger impact on NOx reductions than particulate matter (PM2.5, PM10)**, indicating that additional measures (e.g., industrial emission controls) might be necessary.
   - Future work should explore **long-term monitoring** and evaluate broader socio-economic impacts, including **health benefits, economic activity, and mobility trends**.



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

