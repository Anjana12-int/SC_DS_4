# UK Traffic Accident Analysis

This repository contains an analysis of UK traffic accident data to identify patterns related to road conditions, weather, and time of day, visualize accident hotspots, and determine contributing factors.

## Project Overview

The goal of this project was to explore a dataset of UK traffic accidents and gain insights into the circumstances surrounding them. By analyzing various factors like road surface conditions, weather, light conditions, and time of day, we aimed to understand when and where accidents are more likely to occur and which factors are most influential.
## Dataset
https://www.kaggle.com/api/v1/datasets/download/devansodariya/road-accident-united-kingdom-uk-dataset

## Data

The analysis was performed on a dataset containing information about traffic accidents in the UK. The dataset includes details such as:

- Location (Latitude and Longitude)
- Date and Time of accident
- Accident Severity
- Road Surface Conditions
- Weather Conditions
- Light Conditions
- Number of Vehicles and Casualties
- Other relevant factors

## Analysis and Findings

The analysis involved several steps:

1.  **Data Loading and Exploration**: The dataset was loaded into a pandas DataFrame, and initial exploration was performed to understand the data structure and identify potential issues.
2.  **Data Cleaning and Preprocessing**: Missing values in relevant columns were handled, and the 'Date' and 'Time' columns were processed to extract the hour of the day.
3.  **Pattern Analysis**: The frequency of accidents was analyzed based on Road Surface Conditions, Weather Conditions, Light Conditions, and Hour of Day.
4.  **Accident Hotspot Visualization**: A heatmap was generated using Folium to visualize areas with a high concentration of accidents.
5.  **Contributing Factor Analysis**: A Random Forest Classifier was used to determine the importance of different features in predicting accident severity.

**Key Findings:**

*   The majority of accidents occurred on 'Dry' road surfaces and under 'Fine without high winds' weather conditions.
*   'Daylight: Street light present' had the highest number of accidents, with 'Darkness: Street lights present and lit' being the most frequent condition among dark scenarios.
*   Accidents are least frequent in the early morning (3 am - 5 am) and peak during the afternoon/evening rush hours (3 pm - 6 pm).
*   Geospatial analysis identified areas with a higher density of accidents, indicating accident hotspots.
*   Feature importance analysis showed that 'Hour\_of\_Day' was the most influential factor in predicting accident severity, followed by specific lighting conditions.

## Visualizations

The following visualizations were generated as part of the analysis:

*   Bar plots showing accident counts by Road Surface Conditions, Weather Conditions, and Light Conditions.
*   A line plot showing accident counts by Hour of Day.
*   A heatmap visualizing accident hotspots.
*   A bar plot showing the top feature importances for accident severity prediction.

These visualizations can be found in the notebook.

## Conclusion and Next Steps

The analysis provides valuable insights into the patterns and contributing factors of UK traffic accidents. The findings suggest that focusing accident prevention efforts on identified hotspots during peak accident hours (afternoon/evening rush hour) could be beneficial. Further investigation into the specific characteristics of roads with 'Dry' surfaces and areas with 'Daylight: Street light present' that contribute to the high number of accidents is recommended.

