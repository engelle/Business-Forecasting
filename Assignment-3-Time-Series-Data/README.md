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

## Data Collection Methodology

The data is collected by the **U.S. Census Bureau** through the **Monthly Retail Trade Survey (MRTS)**. The survey collects information about the dollar value of retail sales and end-of-month inventories from a sample of approximately 13,000 retail businesses with paid employees. The sample is drawn from the Census Bureau's Business Register, and businesses are grouped based on factors such as their type of business and sales size.

The survey is conducted **monthly**, with firms in the sample asked to report their sales and inventory data for the month that just ended. The Census Bureau uses reported and estimated data from the sampled businesses to calculate monthly totals. These observations are weighted based on their probability of selection, and the monthly totals are benchmarked to the latest available annual survey totals. The sample is also updated throughout the year to account for new businesses and businesses that are no longer active.

For this assignment, the resulting electronics store retail sales data was accessed through **FRED (Federal Reserve Economic Data)**, maintained by the Federal Reserve Bank of St. Louis.

## Why This Dataset Intrigues Me

This dataset caught my attention because I currently work in retail and wanted to see what retail sales actually look like over time on a larger scale. Since I also have an interest in technology, I chose to focus specifically on electronics stores. I am interested in seeing whether there are noticeable trends or seasonal patterns in the data and how events such as changes in consumer behavior may have affected electronics sales over the past ten years.

## Data Sources

- **Federal Reserve Bank of St. Louis (FRED).** *Retail Sales: Electronics Stores (MRTSSM443142USN).* Data originally provided by the U.S. Census Bureau.  
  https://fred.stlouisfed.org/series/MRTSSM443142USN

- **U.S. Census Bureau.** *Monthly Retail Trade Survey - About the Survey.*  
  https://www.census.gov/retail/mrts/about_the_surveys.html

- **U.S. Census Bureau.** *Monthly Retail Trade and Food Services Survey - Methodology and Technical Documentation.*  
  https://www.census.gov/retail/mrts/how_surveys_are_collected.html
