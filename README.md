# Weather Analytics Dashboard using Power BI, DAX, and Live Weather API 


A production-style **Power BI weather analytics dashboard** built using a **live Weather API**, **Power Query**, and **DAX** to monitor current weather, air quality, and 7-day forecasts across major cities of Nepal.

This project demonstrates end-to-end BI workflow skills including **API integration, JSON transformation, data modeling, DAX development, dashboard design, and insight generation**.

---

## Project Overview

This dashboard was developed to provide a real-time and forecast-based view of environmental conditions in Nepalese cities. It combines live API data with Power BI data modeling and custom DAX measures to create an interactive reporting experience.

The dashboard includes:

- Current weather monitoring
- 7-day temperature forecast
- Rain probability analysis
- Sunrise and sunset timings
- Air Quality Index tracking
- KPI cards for weather metrics
- Best City Insight based on environmental scoring
- Multi-city comparison

---

## Key Features

### Real-Time Weather Monitoring
Tracks current weather conditions for major cities, including:

- Temperature
- Humidity
- Wind speed
- Visibility
- Pressure
- UV index
- Precipitation
- Weather condition

### 7-Day Forecast Analysis
Displays future weather trends with:

- Daily forecast temperatures
- Rain probability by day
- Forecast comparison across cities

### Air Quality Intelligence
Measures and visualizes:

- PM2.5
- PM10
- CO
- NO2
- O3
- SO2

Includes:

- AQI status categorization
- Dynamic DAX-based color coding
- Health suggestion logic

### Best City Insight
Ranks cities based on a weighted score using:

- Lower air pollution
- More comfortable temperature
- Lower rain probability

This feature transforms raw weather data into an actionable insight.

---

## Tech Stack

- **Power BI**
- **DAX**
- **Power Query**
- **REST API**
- **JSON**
- **Data Modeling**

---

## Data Source

Weather data was collected from a live weather API using Power BI's **Web** connector.

### API configuration used
- Forecast: 7 days
- AQI: Yes
- Alerts: No

Data was fetched separately for multiple Nepalese cities and combined into a unified model for analysis.

---

## Cities Included

The dashboard includes major cities of Nepal such as:

- Kathmandu
- Pokhara
- Biratnagar
- Birgunj
- Janakpur
- Dharan
- Lumbini
- Bhaktapur
- Lalitpur

---

## Data Preparation Workflow

1. Generated API response using the Weather API Explorer
2. Connected Power BI to the API using the **Web** connector
3. Fetched weather data for multiple cities by modifying the location parameter
4. Loaded each city as a separate query
5. Combined all city queries into a **Master Table**
6. Created reference tables for:
   - `Current`
   - `Forecast_DAY`
   - `Forecast_Hour`
   - `Location`
7. Removed unnecessary columns
8. Removed duplicates
9. Structured relationships using `Location` as the dimension table
10. Applied DAX measures for business logic and KPI formatting

---

## Data Model

The model is designed using a central **Location** table with one-to-many relationships to:

- `Current`
- `Forecast_DAY`
- `Forecast_Hour`

This structure supports:
- accurate filtering
- reusable city dimension
- scalable reporting logic
- better measure design

---

## DAX Highlights

This project includes custom DAX measures for:

### AQI Logic
- pollutant-based AQI color indicators
- AQI status labels
- health guidance text

### KPI Measures
- current temperature
- average forecast temperature
- humidity
- wind speed
- visibility
- precipitation
- pressure
- UV index
- last updated date and time

### Insight Measures
- city scoring logic
- best city ranking
- dynamic text output for dashboard insight cards
---

## Business Value

This dashboard is more than a weather report. It demonstrates how live external data can be transformed into an analytical product that supports:

- real-time monitoring
- city-level comparison
- environmental awareness
- decision support
- KPI-driven reporting

It also reflects practical BI capabilities relevant to **Data Analyst**, **Business Intelligence**, and **Power BI Developer** roles.
---
## Why This Project Stands Out

This project demonstrates:

- API-to-dashboard pipeline design
- data transformation using Power Query
- dimensional modeling in Power BI
- advanced DAX logic
- user-focused dashboard design
- insight generation from raw environmental data

---

## Author

**Sanjeeb Sapkota**

Data Analytics | Power BI | SAP B1 HANA | SQL

- GitHub: https://github.com/sanjeebsapkota
- LinkedIn: https://www.linkedin.com/in/sanjeeb-sapkota-07b625226/

---

## License

This project is for portfolio and educational purposes.
