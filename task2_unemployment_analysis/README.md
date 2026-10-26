# Unemployment Analysis in India (with Covid-19 Impact)

Analysis of monthly unemployment rates across Indian states from May 2019 to
June 2020. Built for the CodeAlpha Data Science Internship (Task 2).

## Dataset
740 monthly records across 28 regions with Urban/Rural labels. Columns:
region, date, estimated unemployment rate, estimated employed, labour
participation rate, and area. File: `Unemployment in India.csv`.

## Data cleaning
- Removed 28 completely empty rows
- Stripped hidden whitespace from column names and text values
- Converted dates from text (day-month-year) to real datetime values
- Renamed long column names for readability
- Confirmed no missing values remain

## Key findings
- Unemployment held steady at about 9-10% from May 2019 to February 2020.
- After the national lockdown began on 25 March 2020, it more than doubled
  to roughly 24-25% in April and May 2020, then fell to about 12% in June.
- The rise differed sharply by region (Covid period defined as March to June
  2020 against May 2019 to February 2020). Puducherry, Tamil Nadu, Jharkhand
  and Bihar saw the largest increases.
- Urban unemployment was higher than rural throughout (roughly 10-12% against
  7-10% before the lockdown). The gap widened at the peak, with urban reaching
  about 28% against about 21-22% for rural in May 2020, then closed again to
  about 12% for both by June.
- The data covers only 14 months, so true seasonal patterns cannot be
  established. A longer time series would be needed.

## Charts
![Unemployment trend](unemployment_trend%20%281%29.png)

![Covid impact by region](covid_impact_by_region.png)

![Urban vs rural unemployment](urban_vs_rural.png)

## Policy implications
- Target relief at the hardest-hit regions rather than spreading it evenly.
- Urban job support matters, since urban unemployment peaked highest.
- Monthly monitoring can act as an early-warning system for economic shocks.

## Tools
Python, pandas, matplotlib, seaborn, Google Colab
