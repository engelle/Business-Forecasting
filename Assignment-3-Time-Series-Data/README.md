# Assignment #3 - Time Series Data

## Dataset Overview

For this assignment, I selected the **Retail Sales: Electronics Stores** time series from the Federal Reserve Bank of St. Louis (FRED). The original source of the data is the **U.S. Census Bureau's Monthly Retail Trade and Food Services survey**.

The dataset contains monthly estimates of retail sales for electronics stores in the United States. Sales are measured in **millions of dollars** and the data is **not seasonally adjusted**. I selected observations from **January 2016 through December 2025**, giving the dataset 120 monthly observations across a ten-year period.

- **Dataset:** Retail Sales: Electronics Stores
- **FRED Series ID:** MRTSSM443142USN
- **Time Period:** January 2016 - December 2025
- **Frequency:** Monthly
- **Number of Observations:** 120
- **Units:** Millions of Dollars
- **Seasonal Adjustment:** Not Seasonally Adjusted
- **Geographic Coverage:** United States

## Data Dictionary

| Variable | Description | Data Type | Unit/Format |
| --- | --- | --- | --- |
| `observation_date` | The date associated with each monthly retail sales observation. | Date | YYYY-MM-DD |
| `MRTSSM443142USN` | Estimated monthly retail sales for electronics stores in the United States. | Numeric | Millions of U.S. Dollars |
