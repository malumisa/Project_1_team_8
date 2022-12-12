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

Section 2 - The COVID pandemic crisis has forced many small businesses to reassess the decades-old traditional business models or face closing permanently. 
New and existing technologies are thrust to the forefront of every business toolkit, and forward-looking businesses are addressing talent questions that arise from these new digital business skillsets.
We were able to choose a random socioeconomic variables and plot the variations including CAnadian  global retail sales from 2019-2021, Current data on retail sales, umemloyment and sepending data. [PrabhaRS]

Section 3 - In this section we considered different time periods to capture household spending behaviour before and during COVID-19. We carried out regression analysis to test whether the drivers of spending behaviour remained significant over time. Initially, Household final consumption ependiture (HFCE) was considered. Accordingly, HFCE was categorized into food and beverages, food, clothing and footwear, education, transport, food, beverage and accommodation services, accommodation services, and health. Household disposable income (HDI) was the overarching explanatory variable in the analysis. [ S.Malumisa]

## Description of the Data
Section 1 - The Canadian Census is required to be completed by all Canadians every five year.  Focusing on the 2016 and 2021 collection periods would provide a good sense of a before and after that pandemic picture of the Canadian population.  It covers demographic data for a range of socioeconomic variables, and as such lends itself to fruitful analysis.  It is a significantly large data set, which has been made available to developers through an API (https://censusmapper.ca/api).  For the purposes of our work, the StatsCan import package provides the best resource.  It allways the user to download available datasets directly from the StatsCan website directly into the Jupyter Notebook.  Once integrated, the use can create the required DataFrame and data transformation and visualizations.  The two data sets used included, Household income statistics by household type and Impact of the COVID-19 pandemic on income by percentage change in income between 2019 and 2020.  The first provides a demographic breakdown, including income, of the Canadian population by household type.  The second provides statistics on income types and sources for a variety of population pools.  The data is highly coded and downloads as "objects", so a lot of cleaning is required to get it into a codable format.  The type of resulting data works well with bar and line graphs. [Author: M. Carvalh]

Section 2 - The random ecommerce variables we picked were constructed based on
Overall canadian spending (consolidated)
Retaile trade sales by Province and Territory 2021 
Employment ratio 2019-2022
Economic Indicators - Retale sale 2022
[PrabhaRS]

Section 3 - Statistics Canada is a rich source for credible socioeconomic data and can be easily downloadable csv format. For this analysis we made use of  quarterly income and expenditure data for the period q1 2017 -q3 2022. The data was then split into pre-COVID-19 and COVID-19 and we carried out regression analysis to deduce insights on the impact of the pandemic on household spending behaviour.[S. Malumisa]

## Data Sources
Section 1 [M.Carvalho]
* Household income statistics by household type: https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=9810005701
* The impact of the COVID-19 pandemic on income by percentage change in income between 2019 and 2020: https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=9810008701

Section 2 [PrabhaRS]
* Used a user-key parameter to your API calls to authenticate Economic Indicators from The Statcan Daily API
* https://statcan-economic-indicators-statcan-apicast-production.api.canada.ca/v1/ind-econ.json - Data point for API 
* #https://statcan.api.canada.ca/en/detail?api=statcan-economic-indicators#:~:text=Economic%20Indicators%20from%20The%20Statcan%20 - Daily Site
* #https://www150.statcan.gc.ca/n1/dai-quo/ind2-eng.htm - Data view in html
* https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=2010000802&pickMembers%5B0%5D=1.1&cubeTimeFrame.startMonth=01&cubeTimeFrame.startYear=2020&cubeTimeFrame.endMonth=09&cubeTimeFrame.endYear=2022&referencePeriods=20200101%2C20220901
* Retail e-commerce sales - Table: 20-10-0072-01 - release date 2022-11-22 #https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=2010000801&pickMembers%5B0%5D=2.1&pickMembers%5B1%5D=3.2&cubeTimeFrame.startMonth=01&cubeTimeFrame.startYear=2020&cubeTimeFrame.endMonth=09&cubeTimeFrame.endYear=2022&referencePeriods=20200101%2C20220901
* Ecommerce - Retail trade sales by province and territory (x 1,000)
* Retail e-commerce sales - Table: 20-10-0072-01 - release date 2022-11-22 #https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=2010000801&pickMembers%5B0%5D=2.1&pickMembers%5B1%5D=3.2&cubeTimeFrame.startMonth=01&cubeTimeFrame.startYear=2020&cubeTimeFrame.endMonth=09&cubeTimeFrame.endYear=2022&referencePeriods=20200101%2C20220901

Section 3 [S. Malumisa]
* Detailed household final consumption expenditure, Canada, quarterly (x 1,000,000)- SEASONALLY ADJUSTED CONSTANT 2012.  https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=3610012401&pickMembers%5B0%5D=2.2&pickMembers%5B1%5D=3.1&cubeTimeFrame.startMonth=01&cubeTimeFrame.startYear=2010&cubeTimeFrame.endMonth=07&cubeTimeFrame.endYear=2022&referencePeriods=20100101%2C20220701
* Current and capital accounts - Households, Canada, quarterly, - SEASONALLY ADJUSTED AT ANNUAL RATES. https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=3610011201

## Observations

### Before COVID
Section 1 - The 2016 Census collects income levels from the prior year income tax.  Across the household types, the median after tax income was $74,000.00.  In 2016, the smallest contributor to household disposable income came from government benefits.  Couples with children had a median after-tax income of $103,000 in 2016, while multi-generational census households had a combined after tax income of $107,000. Lone-parent families had a median income of $52,000, while couples without children had a median after-tax income of $74,000. 

Senior families, where the highest income earner was 65 years of age or older, had a median after-tax income of $57,800 in 2016, up 4.7% from 2012. Overall, market income (up 8.7% since 2012) has contributed more to this growth than government transfers. Unattached seniors had a median after-tax income of $26,100 in 2016. [MCarvalho]

Section 2 - E-Commerce
* Retail e-commerce, including sales from both store and non-store retailers, rose 14.7% to $18.0 billion in 2018. 
* Retail e-commerce represented 2.9% of total retail sales, compared with 2.6% in 2017. 
* During the November and December holiday shopping season, retail e-commerce accounted for 3.9% of total retail sales, up from 3.5% in 2017, in part due to strong retail e-commerce sales in November 2018. 
* Approximately one-quarter of retail e-commerce sales took place during the 2018 holiday shopping season.
[PrabhaRS]

Section 3 - Q1 2017 - Q4 2019.
* HFCE: -Strong evidence that HDI influenced spending.
* Food and non alcoholic beverages: Strong evidence that HDI influenced spendingg.
* Food: Strong evidence that HDI influenced spending.
* Clothing and footwear: Strong evidence that HDI influenced spending.
* Education: Strong evidence that HDI influenced spending.
* Transport: Strong evidence that HDI influenced spending.
* Food, beverage and accommodation services: Strong evidence that HDI influenced spending.
* Accommodation services: Strong evidence that HDI influenced spending.
* Health: Strong evidence that HDI influenced spending.
[S. Malumisa]

![image](https://user-images.githubusercontent.com/111699427/206927950-7add8b59-1cba-4324-b48c-2cf7208bcf56.png)
![image](https://user-images.githubusercontent.com/111699427/206927597-ba32978d-0638-4129-8aba-073bf95799dc.png)

### After COVID
Section 1 - The 2020 Census collects income levels showed an increase from the prior census period.  Across the household types, the median after tax income was $79,500.00.  In 2020, the smallest contributor to household disposable income came from self-employed income, with government benefits playing a significantly larger contribution relative to 2016.  Couples with children had a median after-tax income of $114,000 in 2020, while multi-generational census households had a combined after tax income of $125,000. Lone-parent families had a median income of $62,000, while couples without children had a median after-tax income of $79,500. [MCarvalho]

Section 2 - Retail e-commerce sales soar to all-time high:
* Retail e-commerce sales reached a record $3.9 billion in May, a 2.3% increase over April and 99.3% increase over February ($2.0 billion).
* Year over year, e-commerce sales more than doubled—with a 110.8% increase compared with May 2019.
* These record gains in e-commerce occurred as total retail sales experienced record declines.
* The impact of COVID-19 is best highlighted using April data. Retail sales plummeted to $33.9 billion in April, a 29.1% decline from February and a 26.4% decline from April 2019. 
* While e-commerce saw a 63.8% monthly increase in April, in-store sales dropped 25.3% . 
* In May, total retail sales started to recover, reaching $39.3 billion.
[PrabhaRS]

Section 3 - Q1 2020 - Q3 2022:
* HFCE: -No evidence that HDI influenced spending.
* Food and non alcoholic beverages: Weak evidence that HDI influenced spendingng.
* Food: Strong evidence that HDI influenced spending.
* Clothing and footwear: No evidence that HDI influenced spending
* Education: No evidence that HDI influenced spending.
* Transport: No evidence that HDI influenced spending.
* Food, beverage and accommodation services: No evidence that HDI influenced spending.
* Accommodation services: No evidence that HDI influenced spending.
* Health: No evidence that HDI influenced spending
[S. Malumisa]

<img width="344" alt="image" src="https://user-images.githubusercontent.com/111699427/207116651-2bc29f26-9f68-445f-8232-5658d6456339.png">


### Analysis
Section 1 - In 2020, the outbreak of COVID-19 and the corresponding public health measures and pandemic relief programs brought significant changes to the Canadian labour market and income landscape. Employment income consists of wages, salaries and commissions from paid employment and net self-employment income. Fewer Canadians received employment income in 2020 as lower-earning jobs disappeared. Household after-tax income growth accelerated from 2015 to 2020, particularly among families with children, driven by increases in government transfers. After-tax income growth was faster for households with lower incomes, reflecting greater contributions of the Canada Child Benefit and pandemic relief benefits on the incomes of lower-income families. [MCarvalho] (Source: https://www.statcan.gc.ca/en/sc/video/income-profile-canadians) 

<img width="474" alt="Screen Shot 2022-12-11 at 12 43 31 PM" src="https://user-images.githubusercontent.com/115101031/206919740-58a49b03-ded3-4f54-a892-60036e8cc908.png">

Over two-thirds of Canadian adults received income from one or more pandemic relief programs. Benefits from COVID-19 income supports offset losses in employment income among low-wage earners.

<img width="743" alt="Screen Shot 2022-12-11 at 12 45 22 PM" src="https://user-images.githubusercontent.com/115101031/206920687-d20c16fa-df33-449d-9833-da889914c223.png">


Section 2 


![project1-gif](https://user-images.githubusercontent.com/116133856/206926681-f0b05b09-59a8-475d-bc66-75453b312f61.gif)
[PrabhaRS]

Section 3 -
* We wanted to test whether spending behaviour changed as a result of covid-19. We carried out a regression analysis of HDI on HFCE and its components (including Food, Clothing and footwear, Education, Transport, Accommodation services, and health).
* Q1 2017 -Q3 2022 results were not consistent across HFCE and its components. We then split the data pre-COVID-19  and COVID-19 and ran regression equations.
* Precovid-Q1 2017 - q4 2019,  Spending on HFCE and its components was largely driven by HDI. Results are significant, high correlation, correct signs in the relationship between explanatory and explained variables.
* 	Covid- Q1 2020- q3 2022. Food spending is the only component with significant results albeit with a puzzle.
* 	Without a doubt, the impacts of the pandemic on Canadian households have been uneven. Results point to the hardships associated with the pandemic as households' spending on high-contact services was muted as many lost their jobs and consequently income. This also came at a time when households became more conscious about their health and finances, triggering precautionary savings. In a recent survey by Statistics Canada, nearly three in four Canadians reported that rising prices affect their ability to meet daily expenses such as transportation, housing, food, and clothing. As such, many households adjusted their spending habits hence the insignificant impact of HDI to drive spending behaviour in the period q1 2020- q3 2022.
[S. Malumisa]


## Conclusions
Despite high job losses and lengthy lock-downs, the Canadian economy remained resilient over the period covering the start and worst of the COVID-19 pandemic. Businesses and consumers appeared to adapt, incuding benefitting from an unprecedented level of support from the government, which helped offset a sharp drop in labour income. On average Canadians spent about $4,000 less last year, largely because:
* many high-contact services such as travel and entertainment have been shut down
* people are being more cautious about both their finances and their health

As a result, household savings have risen across the country to the tune of $180 billion in the past year, or roughly $5,800 per Canadian.
Overall, the impacts of COVID-19 have been uneven—including those on household savings and spending. (Source: https://www.bankofcanada.ca/2021/03/household-consumption-in-a-pandemic/)

Our research sought to better understand the impact on Canadian household spending behaviour.  Our data and analysus concluded:  
* Demographic data between the 2015 and 2020 census data showed that on average household income increased, but the share of that income from government sources changes between the two collections, with a greater percentage of the household drawing some of their income from government sources.
* COVID-19 had an uneven impact on households spending behaviour. Generally, results suggest that households have become more precautionary with spending as they build savings.


## Further Consideration/Next Steps
There is a need to delve deeper into the analaysis at the provincial and regional levels in order to deduce more insights that can inform policy on measures to stimulate spending.  For example, provinces rolled out lock-down measures (and drew back containment measures) at different times.  The population of each province is different, as is income.  How were these variables manifested in the data.

It will be useful to track whether spending behaviours return to pre-pandemic levels or if Canadians will persist with new learned behaviours with respect to pandemic spending?  With so many Canadian adversely affected, do we see greater caution and increased savings moving forward?

With supply chain issues impacting the availability of certain consumer goods, it might be worthwhile also exploring how supply and demand impacted spending during this period?


## Presentation Slidedeck
https://docs.google.com/presentation/d/1YuyYELPtSM5-attMPaKEkIe50e4IxG3hMymvBZNOZ_4/edit?usp=sharing

## Links (Additional Sources)
* https://search.open.canada.ca/en/od/?od-search-portal=Open+Data&search_text=consumer+spending
* https://www12.statcan.gc.ca/wds-sdw/cpr2016-eng.cfm
* https://www12.statcan.gc.ca/census-recensement/2021/dp-pd/prof/details/page.cfm?Lang=E&GENDERlist=1,2,3&STATISTIClist=1&HEADERlist=0&DGUIDlist=2021A00053520005&SearchText=toronto
* https://www.kaggle.com/datasets/phanhutn/car-sale?resource=download
* https://app.slack.com/client/T0416BF14KU/C04CW4S8344#:~:text=8%3A02%20PM-,https%3A//utorvirtdatap%2Dhwb2609.slack.com/archives/C04D0DD8XA7/p1669773017566149,-stories.td.com
* https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=3610012401&pickMembers%5B0%5D=2.2[…]imeFrame.endYear=2022&referencePeriods=20180701%2C20220701
* https://open.canada.ca/data/en/dataset/89077c3a-cfe1-4b6c-a35f-015cb8688f47
* https://mountainmath.github.io/cancensus/index.html 
