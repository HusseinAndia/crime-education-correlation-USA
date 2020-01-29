# crime-education-correlation-USA


The data we have are for the total number of crimes in the US in 1975 - 2015, and for United States of America education budget in 1976 - 2016.
The main question we want to answer from this visualization is to see if there is correlation between spending on education and the number of crimes in US. Is it effected if US government spending more on education over years  that the number of crimes would be decreased?


## Data source

1. [usa-education-budget-analysis](https://www.kaggle.com/marshallproject/crime-rates)

2. [crime-rates](https://datahub.io/core/usa-education-budget-analysis#resource-data)
   - Data comes from Office of Management and Budget, President’s Budget from white house official website on     
     https://www.whitehouse.gov/sites/whitehouse.gov/files/omb/budget/fy2018/hist05z2.xls
     It consists of useful information about BUDGET AUTHORITY BY AGENCY in the range 1976–2022.
     Gross Domestic Value(GDP) comes from DataHub http://datahub.io/core/gdp/r/gdp.csv since it is regularly updated and includes                       
     all country codes.
     *Note that data in `data/budget.csv` starting 2017, the value is estimate value*
     ### Preparation

     There are several steps have been done to get final data.

     * We extracted budget and gdp data separately
     * We merged and added new column `RATIO` which is calculated by `education expenditure / GDP`


## Conclusion


The plot indicates years of increasing in number of crimes between 1975 and 1993 then it started to decrease. Unlike crimes the budget for education is steadily increasing then there are some years it decrease and finally increase again. The plot indicates that there is a very weak negative correlation as if it there was not any correlation at all. The correlation is -0.0982174.
