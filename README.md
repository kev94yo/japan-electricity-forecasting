# Japan Electricity Forecasting
This project performs forecasting on Japan electricity consumption based on time series data and features.

## Motivation
1. Produce more accurate electricity consumption forecasts
2. Successful predictions can lead to less energy waste
  - Better plans for generating energy supply
  - Meeting customers' energy demand

## Project Outline
The data needed are in the `data` folder.

### EDA.ipynb
Run the `EDA.ipynb` file for data preprocessing and EDA.
- **Data Preprocessing**
  - Added features using datetime and holiday information
  - Concatenated weather data by left joining on the electricity consumption dataset
- **Exploratory Data Analysis (EDA)**
  - Visualized consumption by hour, day, month and year to seek insights on potential patterns
  - Produced heatmap and boxplot to search correlations between holiday and consumption

### Forecast.ipynb
Run the `Forecast.ipynb` file for model training, evaluation and prediction.
- **Model Training, Evaluation**
  1. Ridge Regression: Used to model linear relationships between multiple features and one response
  2. SARIMAX: Used for comparison between traditional time series model and machine learning model
  3. XGBoost: Extreme gradient boosting, a form of boosting ensemble method
- **Prediction**
  - Visualized consumption predictions at an hourly level for the next year
