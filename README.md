# Real Estate Market Assessment
#### by The Very Best Team
## Overview

The-very-best-team elected to focus on what is driving the residential real estate market. We sourced real estate and mortgage rate data through Quandl and unemployment and population data through the US Bureau of Labor Statistics. Followed by running correlations between key prospective drivers to include unemployment rates, mortgage rates and population.

## Approach & Methodology

**Why was this topic selected?**

We shared a general curiosity about what factors drive real estate prices up or down. We chose to focus on Zillow real estate and Freddie Mac mortgage rate data because our research found this information to be readily and abundantly available through Quandl. We added additional unemployment and population data through the US Bureau of Labor Statistics.

The Zillow data set led us to focus on QUESTIONS about home value, sales price, inventory and days-to-sell. The key Indicator ID’s that will be in the scripts are summarized as follows:

**ZALL** - Zillow Home Value Index for all homes
**ISAM** - For Sale Inventory (number of listings on the market)
**NSAM** - Median days to pending (median number of days a listing is on the market)
**SSAM** - Median sale price (median value for listings that sold)
 
We added additional datasets to evaluate or HYPOTHESES about prospective drivers in the residential real estate market:

UNEMPLOYMENT RATE was incorporated because we hypothesized that with fewer people getting paychecks there would be less money being invested into real estate.
MORTGAGE RATES were incorporated because we hypothesized that the cost of borrowing has a significant impact on what people can afford to purchase
POPULATION was incorporated because we hypothesized that Colorado population growth would increase demand for housing and subsequently impact home values and sales indicators

## Key Takeaways

We were able to arrive at satisfactory, but sometimes surprising answers to our question set and hypotheses. Our initial analysis lends itself to additional questions and items to explore. Our key takeaways from this initial project were as follows:

1.      POPULATION is highly correlated to sales pricing and home values
2.      UNEMPLOYMENT RATE is moderately correlated to sales pricing
3.      Surprisingly MORTGAGE RATES are uncorrelated to sales pricing, home values, time-to-sell and for-sale inventory

## Project Initiation

We utilized a live API with Quandl to secure and narrow our initial Colorado real estate data set. Additional information regarding unemployment, mortgage rates and population were merged without main real estate data set to build a master file to drive our assessment.

## Notebook Summary & Locator
- Branch = ba/coding = Home Value assessments
- Branch = cdc/coding = Sales Price assessments
- Branch = pw/coding = Sales Inventory assessments
- Branch = KMR/Coding = Days-to-Pending assessments
- The main Quandl API is represented in the cdc/coding file notebook

## Support

Our TA Talon provide key in ensuring our branch updates were handled successfully.

Please reference the Denver University GitLab repository for class materials and instructions.

### Roadmap
Not applicable

### Contributing
Contributions were made in a collaborative, team-oriented style. The team included Binet Alagic, Cole Comstock, Kent Rodgers and Pete Witwer.

### License
We were able to secure our data without cost to the team.

### Project status
Complete.

## Question: How do population, unemployment rates and interest rates affect home values in Colorado?
 
### Process:

By using the master data file that we created, I was able to narrow it down and focus on only the home value indicator code. The indicator code for the home value data was ZALL. The important step was to change the Year-Month column to datetime format. Once it had the correct format, I was able to sort the date from oldest to newest and use the groupby function. Creating this new data frame, it allowed me to plot the charts and find the correlation coefficients between the variables in question. First, I looked at Colorado as a whole, then created the same data frames that looked at three different cities (Denver, Colorado Springs and Greeley).
                           
### Findings:

The correlation coefficient between unemployment and home value is 0.35, a moderate positive correlation. The correlation coefficient between population and home value is 0.95, a strong positive correlation. And the correlation coefficient between interest rates and home value is -0.18, a weak negative correlation. The trends were the same for the three different cities.
