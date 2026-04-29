## Explanation
For the data ingestion phase, I imported three primary datasets from local storage: Maryland State Grant/Loan records, Average Wage statistics (2014–2024), and a Zip Code lookup table.

The cleaning and transformation process involved:

  * **Data Reshaping**: Converted the wage data from a "wide" format to a "long" format using pivot_longer() to make it compatible with time-series analysis.

  *  **Standardization**: Utilized the janitor package to ensure all variable names followed a consistent snake_case format.

  *   **Data Joins**: Performed a left_join() between the grant records and the Zip Code lookup table to map financial data to specific geographic locations.

  *  **Filtering & Aggregation**: Narrowed the scope to Montgomery County and Prince George's County, then aggregated the total grant amounts by fiscal year to prepare for comparative analysis.

## Tools Used

* **Quarto**: The technical publishing system used to integrate R code and narrative text.

* **RStudio**: The Integrated Development Environment (IDE) used for script development.

* **tidyverse**: An ecosystem of packages (including dplyr and tidyr) used for data manipulation and reshaping.

* **janitor**: Used for automated cleaning of data frame column names.

* **plotly**: Implemented for future generation of interactive web-based visualizations.

## Author 
**Ike Charistan D**












