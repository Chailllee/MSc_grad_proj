# Evaluating the Impact of Ultra Low Emission Zone Policies on Air Quality and Public Transportation Choices in Central London



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
- **Analysis Techniques:** Exploratory Data Analysis (EDA), time-series analysis, and regression modeling.
<p align="center">
   <img src="others/Figure%203%20Data%20processing%20flowchart.png" alt="Data processing flowchart" width="480"/>
</p>
<p align="center">
   <em>Fig.2: This flowchart illustrates the data processing steps, including data collection, missing value interpolation, and Kriging-based spatial interpolation, used to analyze the impact of ULEZ policies in Central London.</em>
</p>


## Key Findings


1. **Significant Reduction in Air Pollution Levels**
   - The **Ultra-Low Emission Zone (ULEZ)** policy led to **notable decreases in Nitric Oxide (NO) and Nitrogen Dioxide (NO2) levels**, especially in the later expansion stages (2021 & 2023).
   - **Westminster, Camden, and Kensington & Chelsea** saw the most substantial improvements in air quality.
   - **PM2.5 and PM10 levels** showed moderate improvement, but further measures may be needed for sustained reductions.

<p align="center">
   <img src="others\time trend NO.png" alt="Time trend of Nitric Oxide (NO) levels" width="46%" style="display: inline-block;"/>
   <img src="others\time trend NO2.png" alt="Time trend of Nitrogen Dioxide (NO2) levels" width="45%" style="display: inline-block;"/>
</p>
<p>
   <em>Fig.3: Time trends of Nitric Oxide (NO) and Nitrogen Dioxide (NO2) levels from 2019 to 2024. The vertical blue dotted line is the distinguishing precedent in this study period. The vertical black dotted line represents the timing location of the detected changed point. The red line is the trend of the air pollutant time series in different periods before and after the ULEZ by the linear regression method, and there is a gray line that is the trend of the air pollutant time series during the Covid-19 pandemic.</em>
</p>


2. **Shift in Public Transport Usage**

   - ULEZ **encouraged higher public transport usage**, with increased ridership in underground stations within the policy zones.
   - Reduction in private vehicle use contributed to overall improvements in **air quality and reduced traffic congestion**.

   <p align="center">
      <img src="3Method\3-2Correlation\Correlation matrices -1.png" alt="Correlation matrices -1" width="29%" style="display: inline-block;"/>
      <img src="3Method\3-2Correlation\Correlation matrices -2.png" alt="Correlation matrices -2" width="10%" style="display: inline-block;"/>
      <p align="center"><em>Fig.4: Correlation matrices showing the relationships between different air quality indicators and traffic data.</em></p>
   </p>

3. **Impact Varied by Implementation Stage**
   - **2019 ULEZ Central Zone Launch**: Initial improvements in NO2 and PM levels, but mixed results due to limited coverage.
   - **2021 Inner Expansion**: Reinforced earlier improvements, with significant NO2 reductions in Southwark and Kensington & Chelsea.
   - **2023 Outer Expansion**: Largest and most consistent decrease in NO and NO2 levels across all regions.

<p align="center">
   <img src="others\diff change 2023.png" alt="Difference in air quality changes in 2023" width="550"/>
</p>
<p align="center">
   <em>Fig.5: Post 2023 ULEZ Outer Expansion. Difference change percentage of detectors’ air quality mean value in central London.</em>
</p>
</p>

4. **Limitations and Future Considerations**
   - Some **regions, like the City of London and Camden, showed smaller improvements**, suggesting baseline pollution levels or external factors may have influenced outcomes.
   - **ULEZ policies had a stronger impact on NOx reductions than particulate matter (PM2.5, PM10)**, indicating that additional measures (e.g., industrial emission controls) might be necessary.
   - Future work should explore **long-term monitoring** and evaluate broader socio-economic impacts, including **health benefits, economic activity, and mobility trends**.


### **Future Work**  

While this study provides key insights into ULEZ’s impact on air quality, further research is needed to refine policy effectiveness:  

- **Spatial & Statistical Analysis**:  Use **K-means clustering** to identify high-pollution zones for **targeted interventions**. Apply **logistic regression** to assess ULEZ’s long-term effectiveness.  

- **Long-Term Monitoring**:  Extend observation in **Camden & City of London**, where improvements were **less significant**. Investigate **Westminster** to address persistent pollution sources.  

- **Pollutant & Vehicle Impact**:  Analyze individual **pollutants (NO₂, PM10, PM2.5)** for more precise mitigation strategies. Study emissions from **HGVs, buses, and private cars** to refine vehicle regulations.  

- **Beyond Air Quality**:  Assess ULEZ’s impact on **public health, congestion, property values, and business activity**.  

Future research should integrate **urban mobility, environmental policy, and socio-economic factors** to **optimize low-emission strategies**.