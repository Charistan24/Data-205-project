# Analysis
**Explanation**

I first loaded the three datasets: Maryland State Grants and Loans data, Maryland Average Wage Per Job data, and a ZIP code lookup table. I then cleaned the column names and standardized formats such as ZIP codes and fiscal years so the datasets could be merged properly.

Next, I used the ZIP code lookup table to assign each grant record to a county. After that, I filtered the data to focus only on Montgomery County and Prince George’s County, since they are two large neighboring counties with different economic outcomes.

I then grouped the grant data by county and fiscal year to calculate the total annual grant amount each county received. This allowed me to compare yearly public funding levels.

After preparing the wage dataset, I reshaped it into long format so that county wage values could be matched by year. I then merged the wage and grant datasets into one final dataframe containing:

* Fiscal Year
* County
* Total Grant Amount
* Average Wage Per Job

I created several visualizations, including bar charts, scatterplots, wage gap charts, and an interactive Maryland funding map. These graphs were used to identify trends and communicate findings clearly.

I then conducted a Pearson correlation test with the null hypothesis that there is no linear relationship between total state funding and average wages.

The results showed:

Montgomery County: strong positive correlation (r = 0.882, p < 0.001)
Prince George’s County: strong positive correlation (r = 0.794, p = 0.0035)

Because both p-values were below 0.05, there is statistically significant evidence that higher grant funding is associated with higher wages in both counties.

I also conducted a paired t-test comparing yearly wages between Montgomery County and Prince George’s County. The null hypothesis stated that the average wage difference between counties equals zero.

The p-value was extremely small (p < 0.001), meaning there is strong statistical evidence that Montgomery County had consistently higher wages during the 2014–2024 period.

This analysis identifies strong associations between state funding and wage growth, although it does not prove that funding directly caused wage increases. Other economic factors may also influence wages.

# Tools Used
* R Studio
* Tidyverse Library
* dplyr / tidyr for cleaning and reshaping data
* ggplot2 for visualizations
* Pearson Correlation Testing
* Paired t-test
* Maryland Open Data Portal datasets
# Author

Ike Charistan D








