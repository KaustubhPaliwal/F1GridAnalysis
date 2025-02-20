# Impact of Grid Position, Circuit, and Weather on F1 Race Winners

## Overview
This project analyzes the relationship between starting grid position, track characteristics, weather conditions, and their combined impact on Formula 1 race outcomes. By leveraging historical race data and weather information, we explore how different factors influence final race positions and winning probabilities.

## Data Sources
- **F1 Race Results**: Historical race data, including grid positions, finishing positions, and track details.
- **Weather Data**: Retrieved via OpenMateo API, including temperature and rainfall conditions for each race.
- **Circuit Information**: Track type, width, and overtaking difficulty factors.

## Key Findings
- **Grid Position Matters**: Pole sitters have a 55% chance of winning, while the probability drops significantly beyond third place.
- **Track Type Effects**: Street and road circuits provide a slight advantage for pole position starters.
- **Weather Impact**: Moderate temperatures (~20-25°C) correlate with the highest win probability (0.6), while rain slightly increases finishing position unpredictability.
- **Additional Insights**:
  - Higher temperatures may lead to more tire graining, increasing pit stops and strategic variability.
  - Rain affects driver visibility and car performance, potentially leading to crashes and poor finishes.
  - Track width and overtaking difficulty (beyond street circuits) influence race results, as seen in Abu Dhabi and Spain.
  - Team dynamics and car performance remain significant, but further data is needed to quantify their effects.

## Methodology
- **Exploratory Data Analysis (EDA)**: Data cleaning, visualization, and initial hypothesis testing.
- **Statistical Analysis**: t-tests, correlation analysis, and regression modeling.
- **Machine Learning**: Linear Regression to predict race outcomes based on grid position, weather, and track type.

## Statistical Insights
- **Linear Regression Model**:
  - R² = 0.39 (39% of variance explained)
  - Grid Position Coefficient: 0.47 (strongest predictor)
  - Rain Coefficient: -0.097 (slight advantage in wet conditions)
  - Street Circuit Coefficient: -0.30 (better performance compared to traditional circuits)
- **T-Test**:
  - T-statistic: -48.97, P-value: 0.0 (statistically significant impact of grid position)
- **Error Metrics**:
  - Mean Squared Error (MSE): 14.76 (high variability due to team strategies, crashes, etc.)

## Future Work
- Incorporate real-time race telemetry and sector timing data.
- Analyze team performance and teammate influence.
- Study the impact of pit stop strategies and tire degradation.
- Utilize more advanced machine learning models (Random Forest, Neural Networks) for better prediction accuracy.
