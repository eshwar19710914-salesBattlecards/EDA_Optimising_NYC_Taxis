# EDA_Optimising_NYC_Taxis

## Project Overview

This project presents an Exploratory Data Analysis (EDA) of NYC Yellow Taxi trip data for 2023.

The objective is to analyse taxi demand patterns across time and locations and derive data-driven insights that can support:

- Fleet routing and dispatch optimisation
- Strategic positioning of taxis across zones
- Understanding passenger demand and occupancy
- Identification of high-demand periods and locations
- Pricing and fare analysis

## Business Objective

The analysis focuses on understanding how taxi demand varies by:

- Hour of the day
- Day of the week
- Pickup and drop-off zones
- Passenger count
- Trip distance
- Fare and fare-per-mile
- Vendor
- Additional charges

The findings are translated into practical recommendations for improving fleet utilisation, reducing passenger waiting time and supporting revenue optimisation.

## Dataset

The analysis uses NYC Yellow Taxi trip records for 2023.

Due to the large size of the original dataset, a 5% sample was selected within each date and hour before combining the monthly data.

The resulting analytical dataset contains approximately 1.9 million sampled trip records.

The raw monthly Parquet files are not included in this repository because of their large size.

## Analysis Performed

The EDA covers:

1. Data preparation and sampling
2. Data quality and cleaning
3. Trip demand by hour and day
4. Pickup and drop-off zone analysis
5. Route and speed analysis
6. Passenger demand and occupancy
7. Fare and fare-per-mile analysis
8. Vendor comparison
9. Distance-based analysis
10. Additional charge analysis
11. Business interpretation and recommendations

## Key Insights

The analysis indicates that:

- Taxi demand varies significantly by time, day and location.
- Late afternoon and evening periods show strong passenger demand, with 18:00 among the busiest hours in the sampled data.
- Passenger demand is concentrated around major airport, business, entertainment and transportation zones.
- Fare-per-mile varies across time, distance and vendor.
- Longer trips generally show lower fare-per-mile values than shorter trips.
- Additional charges are frequently observed during higher-demand periods.

## Business Recommendations

### Routing and Dispatch

Use hourly and zone-level demand patterns to position taxis before peak periods and improve dispatch efficiency.

### Strategic Zone Positioning

Prioritise high-demand airport, business, transportation and entertainment zones while dynamically repositioning idle taxis during changing demand periods.

### Pricing Strategy

Use observed time-, distance- and vendor-level fare patterns to inform pricing decisions while maintaining competitive rates and customer value.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Jupyter Notebook

## Repository Contents

- `EDA_Optimising_NYC_Taxis_RAJESHWARAN_R_S.ipynb` – Complete EDA notebook
- `report/` – Final project report
- `visualisations/` – Selected analysis visualisations
- `data/` – Dataset documentation

## Project Type

Academic / Portfolio Project – Exploratory Data Analysis

**Author:** Rajeshwaran R S
