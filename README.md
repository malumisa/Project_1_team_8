# Project 1: Changing Behaviours During the COVID-19 Pandemic
## Team #8 - Using Data Analytics to Evaluate Behaviours

## Abstract
The coronavirus pandemic left a huge impact on every aspect of human life.  In particular, during the pandemic, a lot of assumptions were made about how people's behaviours may have been impacted by ongoing restrictions and lockdowns.  Focus on spending habits, conventional wisdom and economic analysis assumes that spending would have been impacted in a negative way.  As people isolated and hunkered down in their homes, spending on food, personal items, clothing and entertainement would have been reduced.

The project's objective is to provide both an overview and details confirming this assumption.  The overarching question focuses on how behaviours changed relative to spending and the cost of living in Canada, comparing population and economic data both before and during the pandemic.  

To carry out the research and evaluation, several data sources were pooled, including census data from 2016 and 2021, household income and expenditure data  (through StatsCan), as well as evaluation of the cost of living/consumer index during this period.  The data will be examined in correlation to the demographic and socioeconmic makeup of the Canadian population.  

The following steps will be undertaken:

* Collection of data from a validated sources
* Cleaning of the data to extract only useful information in accordance with our project questions
* Construction of valuable analytics and visualizations
* Measurement of the trends using statistical tools
* Validation (or rejection) of our hypothesis based on the evaluating results from analytical tools

## Research Parameters
* Can we define a meaningful approach to describe and compare the Canadian socioeconomic profile before and during the pandemic?
* Is there evidence that Canadians spent more money relative to their disposable income both before and after the pandemic?
* In what commodities did Canadians spend more? (ie. consumer goods, food, retail.)?
* Is there a correlation between spending and pre/post pandemic spending habits?
* Is there evidence that other factors may have contributed to increases in spending during this period? (ie. correlation is not causation)

## Methodology
In March 2021, Deputy Governor Lawrence Schembri spoke about how COVID-19 had affected household saving and spending patterns.  The Canadian economy remained resilient over the period defined by lockdown measures. Businesses and consumers were largely able to adapt, and the housing market remained robust, even while job losses continued to affect many people, but were largely mitigated by an unprecedented level of fiscal support. This helped offset a sharp drop in labour income.

On average Canadians spent about $4,000 less, largely because:
* many high-contact services such as travel and entertainment were shut down
* people were more cautious about both their finances and their health

As a result, household savings rose across the country to the tune of $180 billion in the 2020-2021, or roughly $5,800 per Canadian.  Overall, the resiliency of consumption comes as a result of Canadians reorienting their purchases towards goods from services. The data indicate that with the exception of the first wave pull-back, goods outlays have been largely detached from pandemic dynamics.  

The resiliency of consumption comes as a result of changing spending patterns by Canadians. Provincial restrictions as well as health worries, resulted in consumers shunning “high-touch” areas of the economy, such as recreation, entertainment, and travel services, and, instead, directing more of their income toward purchasing goods (Source: https://economics.td.com/ca-spending-pandemic).

Our analysis hopes to test this idea against available data for this time period.

## Project Team Approach:
Section 1 - A logical place to begin our analysis would be to review the socio-economic make-up of the Canadian population to get a sense of the compsotion of income by household and the sources of disposable income (after tax income).  This will allow us to gauge how this might impact spending behaviour.  Because of the diversity of the Canadian population, we focused on total values and majority populations to ensure a large and consistent sample size for the data.  Using medians for the data also provided reliable values (rather than a mean which might be skewed by outliers). [M.Carvalho]

Section 2 -

Section 3 - In this section we considered different time periods to capture household spending behaviour before and during COVID-19. We carried out regression analysis to test whether the drivers of spending behaviour remained significant over time. Initially, Household final consumption ependiture (HFCE) was considered. Accordingly, HFCE was categorized into food and beverages, food, clothing and footwear, education, transport, food, beverage and accommodation services, accommodation services, and health. Household disposable income (HDI) was the overarching explanatory variable in the analysis. [ S.Malumisa]

Section 4 -


## Description of the Data
Section 1 - The Canadian Census is required to be completed by all Canadians every five year.  Focusing on the 2016 and 2021 collection periods would provide a good sense of a before and after that pandemic picture of the Canadian population.  It covers demographic data for a range of socioeconomic variables, and as such lends itself to fruitful analysis.  It is a significantly large data set, which has been made available to developers through an API (https://censusmapper.ca/api).  For the purposes of our work, the StatsCan import package provides the best resource.  It allways the user to download available datasets directly from the StatsCan website directly into the Jupyter Notebook.  Once integrated, the use can create the required DataFrame and data transformation and visualizations.  The two data sets used included, Household income statistics by household type and Impact of the COVID-19 pandemic on income by percentage change in income between 2019 and 2020.  The first provides a demographic breakdown, including income, of the Canadian population by household type.  The second provides statistics on income types and sources for a variety of population pools.  The data is highly coded and downloads as "objects", so a lot of cleaning is required to get it into a codable format.  The type of resulting data works well with bar and line graphs. [Author: M. Carvalh]

Section 2 -

Section 3 - Statistics Canada is a rich source for credible socioeconomic data and can be easily downloadable csv format. For this analysis we downloaded quarterly income and expenditure data for the period q1 2010 -q3 2022. This was a workable sample size allowing us to carryout regression analysis and deduce more accurate results. In the analysis the time periods were split into; q1 2010- q3 2022, q1 2017 -q3 2022, q1 2017- q4 2019 and q1 2020- q3 2022
[S. Malumisa]

Section 4 -

## Data Sources
Section 1 [M.Carvalho]
* Household income statistics by household type: https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=9810005701
* The impact of the COVID-19 pandemic on income by percentage change in income between 2019 and 2020: https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=9810008701

Section 2 -




Section 3 -
* Detailed household final consumption expenditure, Canada, quarterly (x 1,000,000)- SEASONALLY ADJUSTED CONSTANT 2012.  https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=3610012401&pickMembers%5B0%5D=2.2&pickMembers%5B1%5D=3.1&cubeTimeFrame.startMonth=01&cubeTimeFrame.startYear=2010&cubeTimeFrame.endMonth=07&cubeTimeFrame.endYear=2022&referencePeriods=20100101%2C20220701
* Current and capital accounts - Households, Canada, quarterly, - SEASONALLY ADJUSTED AT ANNUAL RATES. https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=3610011201


Section 4 -


## Observations

### Before COVID
Section 1 - 

Section 2 -

Section 3 -
###q1 2010 - q3 2022
HCFE: r value is 0.87, slope 0.11 pvalue 6.79e-017. There is strong evidence that HDI drove HFCE behavior

###q1 2017 - q3 2022

###q1 2010 - q4 2019

###q1 2020 - q3 2022

Section 4 -

### After COVID
Section 1 - 

Section 2 -

Section 3 -

Section 4 -

### Analysis
Section 1 - 

Section 2 -

Section 3 -

Section 4 -

## Conclusions



## Further Consideration/Next Steps


## Links (Data Sources)
* https://search.open.canada.ca/en/od/?od-search-portal=Open+Data&search_text=consumer+spending
* https://www12.statcan.gc.ca/wds-sdw/cpr2016-eng.cfm
* https://www12.statcan.gc.ca/census-recensement/2021/dp-pd/prof/details/page.cfm?Lang=E&GENDERlist=1,2,3&STATISTIClist=1&HEADERlist=0&DGUIDlist=2021A00053520005&SearchText=toronto
* https://www.kaggle.com/datasets/phanhutn/car-sale?resource=download
* https://app.slack.com/client/T0416BF14KU/C04CW4S8344#:~:text=8%3A02%20PM-,https%3A//utorvirtdatap%2Dhwb2609.slack.com/archives/C04D0DD8XA7/p1669773017566149,-stories.td.com
* https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=3610012401&pickMembers%5B0%5D=2.2[…]imeFrame.endYear=2022&referencePeriods=20180701%2C20220701
* https://open.canada.ca/data/en/dataset/89077c3a-cfe1-4b6c-a35f-015cb8688f47
* https://mountainmath.github.io/cancensus/index.html 
