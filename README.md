# Urban Pulse: NYC Restaurant Inspection Risk

## Project Overview
This project investigates whether NYC ZIP codes with more rodent inspection activity and lower median household income tend to have worse restaurant inspection outcomes.

The unit of analysis is ZIP/ZCTA. The notebook merges:
1. DOHMH New York City Restaurant Inspection Results
2. NYC Rodent Inspection Data
3. ACS 2024 5-Year Median Household Income by ZCTA

## Research Question
Do rodent activity and neighborhood income help explain or predict restaurant inspection outcomes in NYC?

## Hypotheses
- H0: Rodent activity and median household income have no statistically significant relationship with restaurant inspection outcomes.
- HA: Higher rodent activity and/or lower median household income are associated with worse restaurant inspection outcomes.

## Repository Structure
```text
urban-pulse-nyc-restaurant-risk/
├── README.md
├── requirements.txt
├── urban_pulse_milestone2.ipynb
└── output/
    └── generated after running the notebook
```

## How to Run
1. Open `urban_pulse_milestone2.ipynb` in Google Colab or Jupyter.
2. Run all cells from top to bottom.
3. The notebook downloads the datasets directly from public URLs.
4. Generated plots and the top-risk ZIP table are saved in the `output/` folder.

## Main Methods
- Exploratory Data Analysis
- Correlation heatmap
- Bivariate scatter plots and box plots
- Welch's t-test
- Pearson correlation test
- Linear Regression
- Random Forest Regression
- RMSE, MAE, and R² model evaluation

## Data Sources
- DOHMH New York City Restaurant Inspection Results: https://data.cityofnewyork.us/api/views/43nn-pn8j/rows.csv?accessType=DOWNLOAD
- NYC Rodent Inspection Data: https://data.cityofnewyork.us/api/views/frm2-tra7/rows.csv?accessType=DOWNLOAD
- ACS 2024 Median Household Income: https://api.census.gov/data/2024/acs/acs5?get=NAME,B19013_001E&for=zip%20code%20tabulation%20area:*
