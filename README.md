# Air Quality Data Analysis with Amazon PartyRock

## Summary
I used Amazon PartyRock, AWS's no-code generative-AI app builder that runs on Amazon Bedrock, to analyze a 32-day air-quality dataset covering Dec 1, 2025 to Jan 1, 2026. The dataset tracks six pollutants: PM10, PM2.5, CO, NO2, O3 and SO2. I turned the raw readings into summary tables, comparisons, correlations and daily trends.

TODO Cindy:
- Where does the air-quality data come from (source and location), and can you link or add the raw dataset?
- Which course or program was this for (for example, AWS AI & ML Scholars)?
- Can you add a link to the PartyRock app and screenshots?

## Problem
Raw sensor readings are hard to read at a glance. The goal was to summarize pollutant levels, find which pollutants rise and fall together, and spot daily patterns.

## What the output file contains (`data/air_quality_analysis_tables.csv`)
1. **Summary table**: the average, maximum and minimum level for each pollutant, with its general trend
2. **Correlations between pollutants**, for example PM10 with PM2.5 and CO with NO2
3. **Comparison table**: standard deviation, range and number of measurements (666 to 737 per pollutant)
4. **Daily patterns**: the average, minimum and maximum of each pollutant for each day

## Findings (as shown in the file)
- **Rising pollutants.** PM10, PM2.5, CO and NO2 are marked as increasing over the period. Daily averages in the second half of the period are higher than in the first half.
- **Falling pollutants.** O3 and SO2 are marked as decreasing, and SO2 stayed close to zero throughout.
- **Traffic and combustion signal.** CO and NO2 are strongly correlated (0.903), which suggests a shared combustion or traffic source.
- **Ozone pattern.** Ozone moves opposite to NO2 (-0.787) and CO (-0.753), which fits the known pattern of ozone being consumed where nitrogen oxides are high.
- **Peaks.** PM10 reached its maximum of 106 µg/m³ on Dec 18, 2025. PM2.5 reached its maximum of 39.9 µg/m³ on Jan 1, 2026, the highest-pollution day overall, which may be linked to New Year activity.

Note: the file labels the daily section as a "30-day period," but it actually covers 32 days.

## Results
**Results: rerun in progress — real results from my AWS account coming soon.**

## Tools and skills
Amazon PartyRock and Bedrock generative AI, prompt-driven data analysis, descriptive statistics, correlation analysis, time-series trend reading, and turning data into insights.
