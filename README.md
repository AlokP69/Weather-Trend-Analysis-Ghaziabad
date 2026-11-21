# Weather Trend Analysis of Ghaziabad (2015-2024)

## Objective
To study how temperature and rainfall changed over time in Ghaziabad, and to find the monthly and yearly patterns in the weather using Python and Pandas.

## Dataset
- **Source:** Open-Meteo Historical Weather API (daily data for Ghaziabad, 28.67°N, 77.42°E)
- **Period:** 1 January 2015 to 31 December 2024 (3653 days)
- **Variables:** maximum, minimum and mean temperature, rainfall, maximum wind speed
- **Changes made to the dataset:**
  - Renamed columns to shorter names (`temp_max`, `temp_min`, `temp_avg`, `rain_mm`, `wind_max`)
  - Converted the `date` column to datetime format
  - Added new columns: `year`, `month`, `temp_range`, `is_rainy` and `temp_category`
- The dataset had no missing values (checked using `isnull().sum()`), so no cleaning was needed.

## Tools Used
- Python
- Pandas and NumPy (data handling and analysis)
- Requests (to download the data from the API)
- Microsoft Excel (formulas, filter, pivot table, conditional formatting)
- Google Colab and GitHub

## Key Findings
- June is the hottest month (about 32.8°C) and January is the coldest (about 12.7°C).
- Yearly average temperature stayed between 23.6°C (2020) and 24.94°C (2016), with no steady warming trend.
- About 35% of days (1293 of 3653) recorded some rainfall.
- Moderate days (18-30°C) were the most common at about 54%, followed by cold days (24%) and hot days (22%).

## Conclusion
Ghaziabad's weather is driven mainly by the season. The hot summer, monsoon rain and cold winter repeat every year, while the change in average temperature from year to year is small.

## Files in this Repository
- `Ghaziabad_Weather_Trend.ipynb`: main Colab notebook
- `ghaziabad_weather_raw.csv`: original data downloaded from the API
- `ghaziabad_weather_edited.csv`: data with the new columns

  Alok Pandey
  2026B01010074
  CSE-02
