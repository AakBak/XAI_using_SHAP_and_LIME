# XAI_using_SHAP_and_LIME

# Predicting Bike Sharing Demand

🚴 Welcome to the Bike Sharing Demand Prediction project! 🚴

## Overview

In our journey to predict bike sharing demand, we followed a meticulous, data-driven process. We began by preparing the dataset, engineering features such as date components, temperature, and weather conditions. Categorical variables were transformed, and numerical features standardized for consistency.

## Model Selection and Tuning

For the regression task, we selected the robust XGBoostRegressor, known for its prowess. Hyperparameter tuning further optimized the model's predictive power. During training, we closely monitored performance with an evaluation set.

## Model Evaluation

The fruits of our labor were revealed during model evaluation, where we achieved an impressive RMSE (Root Mean Square Error) of 0.0884, a testament to the model's accuracy.

## Feature Importance and Interpretability

Delving deeper into feature importance, we uncovered insights into the factors influencing bike rental counts. Additionally, we used Lime and SHAP values to illuminate individual predictions, unraveling the intricate web of feature contributions.

## Two-Step Regression Process

In a separate process, we performed a two-step approach to predict 'casual' and 'registered' user counts in a bike-sharing system. Normalizing target variables and training XGBoost regression models resulted in low RMSE values (0.1727 for 'casual' and 0.0909 for 'registered'), indicating strong predictive performance.

With these insights and predictive models, we stand ready to unlock the secrets of bike sharing demand.
 
# Bike Sharing Dataset

## Background

Bike sharing systems represent a new generation of automated bike rentals, contributing to traffic, environmental, and health solutions. With over 500 programs globally and 500,000 bicycles, these systems generate valuable data for research. Unlike traditional transport services, bike sharing records explicit travel details, forming a virtual sensor network for city mobility.

## Dataset

The dataset includes a two-year historical log (2011-2012) from the Capital Bikeshare system in Washington D.C., USA. Aggregated on hourly and daily bases, the dataset incorporates environmental and seasonal information, such as weather conditions, precipitation, day of the week, and more.

## Associated Tasks

1. **Regression:**
   Predict bike rental count hourly or daily based on environmental and seasonal settings.

2. **Event and Anomaly Detection:**
   Bike rental counts correlate with town events, traceable through search engines. The data is suitable for validating anomaly or event detection algorithms.

## Files

- `Readme.txt`
- `hour.csv`: Bike sharing counts aggregated on an hourly basis. Records: 17,379 hours
- `day.csv`: Bike sharing counts aggregated on a daily basis. Records: 731 days

## Dataset Characteristics

Both `hour.csv` and `day.csv` contain the following fields:

- `instant`: record index
- `dteday`: date
- `season`: season (1:spring, 2:summer, 3:fall, 4:winter)
- `yr`: year (0: 2011, 1:2012)
- `mnth`: month (1 to 12)
- `hr`: hour (0 to 23)
- ... (and more)

## License

Use of this dataset in publications must be cited to the following publication:

[Event labeling combining ensemble detectors and background knowledge](http://dx.doi.org/10.1007/s13748-013-0040-3)

Fanaee-T, Hadi, and Gama, Joao. "Progress in Artificial Intelligence" (2013): pp. 1-15, Springer Berlin Heidelberg, doi:10.1007/s13748-013-0040-3.

## Contact

For further information about this dataset, please contact Hadi Fanaee-T (hadi.fanaee@fe.up.pt).

Feel free to explore the data and contribute to the community! 🚀