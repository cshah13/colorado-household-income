# colorado-household-income
An analysis of factors impacting average household income throughout Colorado.
## Background Information
This analysis aims to use simple and multiple linear regressions to understand factors impacting household income in Colorado. 

Household income in the Denver Metro area has been rapidly increasing according to [The Denver Business Journal](https://www.bizjournals.com/denver/news/2020/12/24/denvers-average-income-keeps-growing.html). The biggest jump was between 2018-2019. Despite the pandemic, the average household income is predicted to continue growing. However, an article in the [Denver Post](https://www.denverpost.com/2020/12/07/colorado-may-not-recover-jobs-lost-this-year-until-2023-c-u-forecasters-predict/) indicates that Colorado lost nearly 149,000 jobs in 2020. A different article in the [Denver Post](https://www.denverpost.com/2018/01/05/forget-middle-class-in-denver-it-takes-63000-a-year-for-a-family-to-just-subsist/) discusses the high cost of living in Colorado that is hindering people from paying for basic neccesities. It is clear that different areas in Colorado are facing different experiences and economic situations. This project aims to understand different factors that contribute to the average household income in different tracts in Colorado.

## Business Question
What factors contribute to different average household incomes in tracts in Colorado?

## Open Data
This analysis uses open data from [The Opportunity Atlas](https://opportunityatlas.org) which provides social mobility data from 20 million anonymous individuals. 
The following data sets were used for this analysis. All original data can be found [here](https://github.com/cshah13/colorado-household-income/blob/main/Original%20Data.xlsx)
- Household Income (average household income from 2014-2015)
- Employment Rate (fraction who have positive earnings in 2015)
- Density of Jobs in 2013 (number of jobs per square mile in 2013)
- Median Rent (median rent between 2012-2016)

## Data Analysis Questions
Microsoft Office Excel will be used to conduct simple and linear regressions to answer the following data questions:
1. How do employment rates impact average household income in Colorado tracts?
2. How do employment rates, median rent, and number of jobs per square mile impact average houshold income in Colorado tracts?

## Simple Linear Regression Data Answer
### How do employment rates impact average household income in Colorado tracts?
The simple linear regression indicates the relationship between average household income and employment rates to be __Average Household Income = -42826.304 + 111888.601(Employment Rate)__. This means that for every 1% increase in a tract's employment rate, the average household income increases by $1,118.89. The F significance/p-value of 2.0082E-37 is below 0.05, indicating that we reject the null hypothesis that there is no relationship between average household income and employment rates, and there is a significant relationship between the two factors. However, the R Squared value indicates that only 35.7% of the data fits the regression model. The standard error of 8461.327 indicates that 95% of our data is within 16,922.654 and the rest can be considered outliers. The graph below shows the actual and predicted data. There were only 373 tracts in the data analysis, so an increase in the sample number could lead to more precise outcomes. The complete data analysis can be found [here](https://github.com/cshah13/colorado-household-income/blob/main/Data%20Analysis.xlsx).
![alttext](https://github.com/cshah13/colorado-household-income/blob/main/Simple%20Linear%20Regression%20Graph.png)

## Multiple Linear Regression Data Answer
### How do employment rates, median rent, and number of jobs per square mile impact average houshold income in Colorado tracts?
The multiple linear regression provides information about the relatonship between average household income and employment rates, median rent, and number of jobs per square mile. The relationship is __Average Household Income = -46877.601 + 0.021(Number of Jobs per Square Mile) + 102238.347(Employment Rate) + 9.877(Rent)__. This means that for every additional job present per square mile in a tract, the household income in the tract increases by 0.021. For every 1% increase in employment rate, the household income increases by $1,022.38. For every one dollar increase in monthly rent, the houshold income increases by $9.877. Both employment rate and rent have F significance/p-values less than 0.05, indicating that we reject the null hypothesis that there is no relationship between the variables and average household income, and the variables are significant. However, the number of jobs present per square mile has an F significance/p-value greater than .05, indicating that we cannot reject the null hypothesis that there is no relationship between average household income and number of jobs, so this variable may not have a strong relationship with household income. The R Squared value indicates that only 44.79% of the data fits the regression model. The standard error of 7859.6 indicates that 95% of the data is within 15,719.2 and the rest can be considered outliers. There were only 373 tracts included in this analysis, so increasing that value could lead to more precise results. The complete data analysis can be found [here](https://github.com/cshah13/colorado-household-income/blob/main/Data%20Analysis.xlsx).

## Business Answer
The simple linear regression model indicates that employment rates within each tract are a significant factor impacting average household income throughout Colorado. The multiple linear regression indicates that median rent is also a factor impacting household income throughout Colorado. Possible reasons for this could be that people are working more to be able to cover the cost of rent. The multiple linear regression also analyzed the number of jobs per square mile. There was not a significant relationship between the number of jobs per square mile and the average household income. A potential reason for this could be that people commute to different locations to work. A multiple linear regression could be conducted in the future without the number of jobs per square mile; this will allow us to identify the relationship solely between household income and the statistically significant values. Since both regression models had low R Squared values, I am not confident that household income can be accurately predicted using these metrics, but general trends can still be visualized. This analysis only analyzed 373 tracts, so more data will be neccesary to have precise conclusions. In the future, indicators such as education rates and health outcomes can be analyzed to identify potential relationships with household income. This information is important to understand areas of development needed in the state. For example, since employment rates are related to household income, organizations can implement programs to increase employment rates in communities. These programs could include job application workshops and interview preperation tools. This information will be useful to both government and nonprofit organizations working to improve social mobility in Colorado. Although the analysis can be used to identify factors that need to be addressed, deeper analysis is neccesary to make accurate conclusions.

## Step by Step Instructions
1. Downloaded Colorado household income data, employment data, rent data, and number of jobs per square mile data from the Opportunity Atlas
2. Used V-LOOKUP to reorganize the important information into one spreadsheet
3. Used the Excel Data Analysis ToolPak regression function to conduct a simple linear regression analysis for household income and employment rate
4. Used the scatterplot function to create a visualization for the linear regression
5. Used the Excel Data Analysis ToolPak regression function to conduct a mulitple linear regression analysis for household income, employment rate, number of jobs per square mile, and rent

