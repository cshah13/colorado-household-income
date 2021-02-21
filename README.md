# colorado-household-income
An analysis of factors impacting average household income throughout Colorado
## Background Information
This analysis aims to use simple and multiple linear regressions to understand factors impacting household income in Colorado. 

Household income in the Denver Metro area has been increasing according to [The Denver Business Journal](https://www.bizjournals.com/denver/news/2020/12/24/denvers-average-income-keeps-growing.html). Despite the pandemic, the household income is predicted to continue growing. An article in the [Denver Post](https://www.denverpost.com/2018/01/05/forget-middle-class-in-denver-it-takes-63000-a-year-for-a-family-to-just-subsist/) discusses the high cost of living in Colorado that is hindering people from paying for basic neccesities. This project aims to understand different factors that contribute to the average household income in different tracts in Colorado.

## Business Question
What factors contribute to different household incomes in tracts in Colorado?

## Open Data
This analysis uses open data from [The Opportunity Atlas](https://opportunityatlas.org) which provides social mobility data from 20 million anonymous individuals. 
The following data sets were used for this analysis. All original data can be found [here](https://github.com/cshah13/colorado-household-income/blob/main/Original%20Data.xlsx)
- Household Income (average household income from 2014-2015)
- Employment Rate (fraction who have positive earnings in 2015)
- Density of Jobs in 2013 (number of jobs per square mile in 2013)
- Median Rent (median rent between 2012-2016)

## Data Analysis Questions
Microsoft Office Excel will be used to conduct simple and linear regressions to answer the following data questions:
1. How do employement rates impact household income in Colorado tracts?
2. How do employement rates, median rent, and job density impact houshold income in Colorado tracts?

## Simple Linear Regression Data Answer
### How do employement rates impact household income in Colorado tracts?
The simple linear regression indicates the relationship between household income and employment rates to be __Household Income = -42826.304 + 111888.601(employement rate)__. This means that for every 1% increase in a tract employement rate, the houshold income increases by $1,118.89. The F significance and p-value of 2.0082E-37 is below 0.05, indicating a significant relationship between the two factors. However, the R Squared value indicates that only 35.7% of the data fits the regression model. The standard error of 8461.327  indicates that 95% of our data is within 16,922.654 and the rest can be considered outliers. The graph below shows the actual and predicted data. There were only 373 tracts in the data analysis, so an increase in this number could lead to more precise outcomes. The complete data analysis can be found [here](https://github.com/cshah13/colorado-household-income/blob/main/Data%20Analysis.xlsx)
![alttext](https://github.com/cshah13/colorado-household-income/blob/main/Simple%20Linear%20Regression%20Graph.png)

## Multiple Linear Regression Data Answer
### How do employement rates, median rent, and job density impact houshold income in Colorado tracts?

## Business Answer

## Step by Step Instructions


