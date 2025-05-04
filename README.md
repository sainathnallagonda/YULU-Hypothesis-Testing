# Yulu Bike Sharing Analysis - Hypothesis Testing

## Project Overview

This project analyzes bike sharing data from Yulu to understand usage patterns and factors affecting bike rental demand. The analysis employs statistical hypothesis testing to identify significant relationships between various factors and bike rental counts.

## Dataset Description

The dataset contains 10,886 records with 12 columns including:
- `datetime`: Date and time of the record
- `season`: Season (1=spring, 2=summer, 3=fall, 4=winter)
- `holiday`: Whether the day is a holiday (0=no, 1=yes)
- `workingday`: Whether the day is a working day (0=no, 1=yes)
- `weather`: Weather condition (1=clear, 2=cloudy/mist, 3=light rain/snow, 4=heavy rain/snow)
- `temp`: Temperature in Celsius
- `atemp`: "Feels like" temperature in Celsius
- `humidity`: Relative humidity
- `windspeed`: Wind speed
- `casual`: Number of casual users
- `registered`: Number of registered users
- `count`: Total number of bike rentals (casual + registered)

##  Hypothesis Testing

The project tested several key hypotheses:

- **Weekday vs. Weekend Bicycle Demand**:
  - H₀: No significant difference in bike rides between weekdays and weekends
  - H₁: Significant difference exists between weekdays and weekends
  - Result: Failed to reject null hypothesis (p-value = 0.226)

- **Weather Conditions and Bicycle Demand**:
  - H₀: Bicycle demand is the same across different weather conditions
  - H₁: Bicycle demand differs significantly across weather conditions
  - Result: Rejected null hypothesis (p-value = 5.48e-42)

- **Seasonal Bicycle Demand**:
  - H₀: Bicycle demand is the same across different seasons
  - H₁: Bicycle demand differs significantly across seasons
  - Result: Rejected null hypothesis (p-value = 6.16e-149)

- **Weather Conditions across Seasons**:
  - H₀: Weather conditions are distributed similarly across seasons
  - H₁: Weather conditions differ significantly across seasons
  - Result: Rejected null hypothesis (p-value = 1.55e-07)

##  Key Findings

1. **No significant difference** in bicycle demand between weekdays and weekends
2. **Weather significantly impacts demand**:
   - Highest demand in clear weather (mean = 205.24)
   - Lowest in light rain/snow (mean = 118.85)
3. **Strong seasonal variations** in bicycle rental patterns
4. **Weather conditions vary significantly** across different seasons

##  Business Implications

1. **Weather-Based Strategies**: Implement dynamic pricing or inventory management based on weather forecasts
2. **Seasonal Planning**: Develop season-specific marketing campaigns and resource allocation
3. **Consistent Weekday/Weekend Service**: Maintain similar operational levels throughout the week
4. **Predictive Forecasting**: Use weather-season relationships for improved demand prediction

##  Tools & Technologies

- Python (Pandas, NumPy)
- Statistical testing (SciPy)
- Data visualization (Matplotlib, Seaborn)
- Hypothesis testing methodologies
