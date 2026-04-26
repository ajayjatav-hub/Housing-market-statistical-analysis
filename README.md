# Housing-market-statistical-analysis
🏠 U.S. Housing Market Statistical Analysis (2005–2013)
Overview
This project conducts a statistical analysis of the U.S. housing market using data from the American Housing Survey (AHS) for the years 2005, 2007, 2009, 2011, and 2013. The central focus is to examine whether market values differ between occupied and not-occupied housing units, and whether any such differences follow a discernible pattern over time.

Research Questions

Are there statistically significant differences in the market values of occupied versus not-occupied housing units?
Do these differences follow a pattern over the period 2005 through 2013?


Dataset

Source: American Housing Survey (AHS)
Years Covered: 2005, 2007, 2009, 2011, 2013
Scope: U.S. housing units, segmented by occupancy status
The dataset was cleaned and pre-processed prior to analysis to ensure consistency and usability across all survey years.


Methodology

Statistical Test: Independent samples t-distribution (t-test) applied separately for each survey year to compare mean market values between occupied and not-occupied units.
Visualisation: Histograms were generated for each year to illustrate the distribution of market values across both occupancy groups.
Tool Used: Microsoft Excel


Note: This analysis can equivalently be reproduced in a Jupyter Notebook using Python (e.g., scipy.stats, pandas, matplotlib).


Key Findings
Question 1 — Significance of Differences
| Year | Significant Difference? | Direction               |
|------|------------------------|-------------------------|
| 2005 | Yes                    | Occupied > Not-Occupied |
| 2007 | No                     | No significant difference |
| 2009 | No                     | No significant difference |
| 2011 | Yes                    | Occupied > Not-Occupied |
| 2013 | No                     | No significant difference |
The difference in market values is statistically significant only for 2005 and 2011, with occupied units carrying a higher market value in both years. For the remaining years (2007, 2009, 2013), no statistically significant difference was observed.
Question 2 — Pattern Over Time
A consistent directional pattern emerges across all five years: the market value of occupied units is never less than that of not-occupied units. In years where a significant difference exists (2005, 2011), occupied units command higher values; in the remaining years, the two groups are statistically comparable.

Summary Pattern: Occupied ≥ Not-Occupied across all surveyed years.


Repository Structure
├── data/               # Cleaned datasets for each survey year
├── analysis/           # Excel workbooks with t-tests and histograms
└── README.md

Tools & Technologies
ToolPurposeMicrosoft ExcelData analysis, t-tests, histogram visualisationAmerican Housing SurveyPrimary data source

Future Work

Reproduce the analysis in a Jupyter Notebook using Python for greater reproducibility and automation.
Extend the analysis to include additional variables (e.g., housing type, region, income bracket).
Apply regression modelling to control for confounding factors affecting market value.


Author
Ajay_Jatav
License
This project is for educational and analytical purposes. Data sourced from the U.S. Census Bureau's American Housing Survey.
