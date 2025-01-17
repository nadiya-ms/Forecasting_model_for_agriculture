# Forecasting model for agriculture supervised ML

## Project Overview

Assessing soil condition through metrics like nitrogen, phosphorus, potassium levels, and pH is crucial for understanding soil health. However, the process can be both costly and time-intensive, often requiring farmers to prioritize specific measurements based on their budget limitations.

When selecting crops to plant each season, farmers must weigh several factors to achieve the highest possible yield. Among these, soil condition plays a critical role in crop growth. Key elements such as nitrogen and potassium levels are essential for determining soil suitability. Since each crop thrives under specific soil conditions, maintaining optimal levels of these elements is vital to ensuring healthy growth and maximizing productivity.

A farmer approached a machine learning expert, seeking assistance in identifying the most suitable crop for their field. Due to budget constraints, the farmer explained that they could only afford to analyze one of the following four essential soil properties:

*   `Nitrogen` content in the soil
*   `Phosphorous` content in the soil
*   `Potassium` content in the soil
*   `Soil pH` value

Recognizing this as a feature selection challenge, I set out to determine which single feature would provide the highest accuracy in predicting the appropriate crop and has the strongest predictive performance. The goal was to help the farmer make an informed decision via cration of multi-class classification model.

## Project Objective

The task was to identify the single soil property that provided the most reliable predictive performance for classifying crop types. The dataset called `soil_measures.csv` contains:

- `"N"`: Nitrogen content ratio in the soil
- `"P"`: Phosphorous content ratio in the soil
- `"K"`: Potassium content ratio in the soil
- `"pH"` value of the soil
- `"crop"`: categorical values that contain various crops (target variable).

Each row in this dataset represents various measures of the soil in a particular field. Based on these measurements, the crop specified in the `"crop"` column is the optimal choice for that field.  
The dataset was analyzed to determine which feature achieved the highest predictive score for the `"crop"` variable.

Based on the analysis, a variable named `best_predictive_feature` was created and formatted as a dictionary.

The dictionary was designed to include the name of the most predictive feature as the key and its evaluation score (based on the chosen metric) as the value.


