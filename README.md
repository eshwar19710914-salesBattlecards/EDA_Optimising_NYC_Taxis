# EDA_Optimising_NYC_Taxis

## Exploratory Data Analysis of NYC Yellow Taxi Trips

This project presents an Exploratory Data Analysis (EDA) of **NYC Yellow Taxi trip data for 2023**.

The objective is to analyse taxi demand patterns across **time, day, location, passenger behaviour and fare characteristics**, and translate the findings into practical recommendations for taxi fleet operations.

---

## Business Objective

The analysis focuses on identifying data-driven opportunities to support:

- Fleet routing and dispatch optimisation
- Strategic positioning of taxis across zones
- Identification of high-demand periods and locations
- Understanding passenger demand and occupancy
- Fare and pricing analysis
- Improved fleet utilisation and reduced idle time

---

## Dataset

The analysis uses the **2023 NYC Yellow Taxi Trip Records**.

The original dataset consists of monthly Parquet files covering January to December 2023.

Due to the size of the original dataset, a **5% sample was selected within each date and hour** before combining the monthly data for analysis.

### Sampled Dataset

- Period: January–December 2023
- Sampling approach: 5% within each date and hour
- Final analytical sample: approximately **1.9 million trip records**
- Sampling was performed consistently across dates and hours to retain temporal demand patterns.

The original large Parquet files are not included in this repository.

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Jupyter Notebook

---

## Key Analysis Areas

The EDA covers:

### 1. Data Preparation & Cleaning
- Monthly data sampling and consolidation
- Missing-value analysis
- Data quality checks
- Feature preparation and derived variables

### 2. Demand Analysis
- Trips by hour
- Trips by day
- Weekday vs weekend patterns
- Pickup and drop-off zone analysis
- High-demand locations
- Passenger demand and occupancy

### 3. Route & Zone Analysis
- Pickup/drop-off patterns
- Zone-level demand
- Traffic concentration
- Route speed analysis
- High-traffic zones

### 4. Fare & Revenue Analysis
- Fare per mile
- Fare patterns by hour and day
- Vendor-level fare comparison
- Distance-tier fare analysis
- Passenger and fare characteristics
- Extra-charge patterns

---

## Key Insights

The analysis indicates that taxi demand varies significantly by **time, day and location**.

### Demand Patterns

- Taxi demand increases during daytime and reaches its highest levels during the **late afternoon and evening**.
- **18:00** was identified as the busiest hour in the sampled data.
- Early morning hours, particularly around **05:00**, show substantially lower demand.
- Passenger demand is also influenced by the day of the week, with higher demand observed on weekends in several measures.

### Zone-Level Demand

Passenger and trip volumes are concentrated in important transportation, business and entertainment locations.

High-demand areas identified in the analysis include:

- JFK Airport
- LaGuardia Airport
- Midtown Center
- Upper East Side South
- Upper East Side North
- Times Sq/Theatre District
- Midtown East
- Penn Station/Madison Sq West

### Fare Patterns

Fare per mile varies across:

- Time of day
- Day of week
- Trip distance
- Taxi vendor

The analysis also indicates that **fare per mile generally decreases as trip distance increases**, highlighting differences in fare economics across distance tiers.

### Extra Charges

Extra charges occur frequently in the sampled dataset, with approximately **62% of sampled trips** having an extra charge.

The frequency of extra charges varies across both **hours and pickup zones**, with higher frequencies observed during several late-afternoon and evening periods.

---

## Business Recommendations

### 1. Optimise Routing & Dispatch

Increase taxi availability ahead of peak periods and use historical zone-hour demand patterns to support proactive dispatching and vehicle repositioning.

### 2. Strategic Zone Positioning

Position taxis around high-demand transportation hubs, business districts and other consistently busy zones during their respective peak periods.

During lower-demand periods, vehicles can be rebalanced toward locations where demand is expected to increase.

### 3. Data-Driven Pricing

Use observed **time-, distance- and vendor-level fare patterns** to inform pricing decisions while maintaining competitive rates and customer value.

### 4. Improve Fleet Utilisation

Combine demand, passenger occupancy, route speed and zone-level insights to reduce idle time and improve vehicle utilisation.

---

## Project Deliverables

### Jupyter Notebook

The notebook contains the detailed Python-based analysis, data preparation, calculations and visualisations.

**File:**

`EDA_Optimising_NYC_Taxis_RAJESHWARAN_R_S.ipynb`

### Final Report

The PDF report contains the analysis findings, visualisations, interpretations and business recommendations.

**Location:**

`report/EDA_NYC_Taxi_Analysis_RAJESHWARAN R S.pdf`

---

## Important Assumption

The analysis is based on a **5% sample taken within each date and hour** of the monthly datasets.

Therefore, trip counts and passenger counts shown in the analysis represent the sampled dataset unless explicitly scaled to estimate the underlying population.

The sampling approach was used to make the large 2023 dataset computationally manageable while retaining representation across dates and hours.

---

## Project Structure

```text
EDA_Optimising_NYC_Taxis/
│
├── README.md
│
├── EDA_Optimising_NYC_Taxis_RAJESHWARAN_R_S.ipynb
│
└── report/
    ├── EDA_NYC_Taxi_Analysis_RAJESHWARAN R S.pdf
    └── README.md
