# World Happiness Report
## Objective:
This project explores multiple factors to see what drives happiness, or unhappiness, both worldwide and regional. Using data from the world happiness report, global country information report, world happiness and inflation report, suicide rate report and life expectancy report, I was able to pull data from several different places and view what drives our happiness.  


## Project Setup Instructions:
+ Fork the repo and clone it to your own computer
+ Load the clone in your code editor
+ Create and activate a virtual environment in that folder
+ Install the "requirements.txt" file
+ Run "world happiness.ipynb"
(If you need to select an environment/kernal to run it in, choose Python > venv. It should have a star next to it.)  
This program does ask for your input at times, so please be mindful of the prompts.  

## Virtual Environment Commands 
| **Command** |           **Windows**                 |            **Linux/Mac**             | 
| ----------  | ------------------------------------- | ------------------------------------ |
|  Create     |    `python -m venv venv`              |   `python3 -m venv venv`             |
|  Activate   |    `source venv/Scripts/activate`     |   `source venv/bin/activate`         |
|  Install    |    `pip install -r requirements.txt`  |   `pip install -r requirements.txt`  |
|  Deactivate |    `deactivate`                       |   `deactivate`                       |


## Project Overview:
This dives into many factors of world happiness, such as mortality, inflation, health cost, freedom of choice and more. 
This project intends to:  
+ Clean and prepare the data to ensure usibility.
+ Group the data by country, year, or comparable groupings to see what does/does not affect happiness.
+ Create charts for visiblity to show outliers or trends leading to happiness/unhappiness.
+ Allow input for the user to see the happiness of a country from 2003-2024 (when available).
+ Allow input for the user to see the inflation rates of a country from 2015-2023 (when available).


## Technologies Used:
Jupyter notebook was used to allow for a narrative-driven presentation of code and charts.  
Pandas was used in conjuction with Python to clean the data. All data is on a relative path.    
Matplotlib and Seaborn were used for charting and visualization purposes.  
IPython clear input was used to clear input in areas, just to make things look nice overall.  
SQlite3 was used for quick handling to join data for querying purposes.  
Gitbash and Github were used for uploading/downloading and viewing purposes (in that order).  
Tableau was used for a finished product view of the project.  
Please run requirements.txt to download the virtual environment and all needed libraries.  


<!-- The world happiness report includes: 
Year
Country Name
Life Ladder (happiness) 
Log GDP per capita 
Social support 
Healthy life expectancy at birth 
Freedom to make life choices 
Generosity 
Perceptions of corruption 






The world happiness index & inflation report includes: Country, Year (2015-2023), Headline Consumer Price Inflation, Energy Consumer Price Inflation, Food Consumer Price Inflation, Official Core Consumer Price Inflation, Producer Price Inflation, GDP deflator Index growth rate, Continent/Region, Score (happiness), GDP per Capita, Social support, Healthy life expectancy at birth, Freedom to make life choices, Generosity, Perceptions of corruption.  
Suicide rate: Country, GDP per capita, Suicide rate (from 2023).  
Life expectancy: Country, Life Expectancy (years) - Men, Life Expectancy (years) - Women, Happiness Score, Fertility Rate (births per woman) (from 2023).  
Global country information dataset: Country, Density, Abbreviation, Agricultural Land( %), Land Area(Km2), Armed Forces size, Birth Rate, Calling Code, Capital/Major City, Co2-Emissions, CPI, CPI Change (%), Currency-Code, Fertility Rate, Forested Area (%), Gasoline Price, GDP, Gross primary education enrollment (%), Gross tertiary education enrollment (%), Infant mortality, Largest city, Life expectancy, Maternal mortality ratio, Minimum wage, Official language, Out of pocket health expenditure, Physicians per thousand, Population, Population: Labor force participation (%), Population: Labor force participation (%), Total tax rate, Unemployment rate, Urban_population, Latitude, Longitude.   

continents2: only the name and subregion columns were used in tableau as a last minute addition.
name: text
subregion: text-->

## Data summary:
**Total records**  
world happiness report: 2363 rows, 11 columns  
life expectancy & suicide rate: 150 rows, 7 columns  
world happiness & inflation report: 1232 rows, 8 columns    
global country information report: 194 rows, 19 columns  

## Basic stats:
All Happiness is on a 1-10 scale over 165 countries over 20 years (2005-2024)  
Happiness mean: 5.48   
Happiness min: 1.28   
Happiness max: 8.01   


## Data sources:
All data sources used during this project are listed below.  Any additional information that I used while researching this project is listed in the personal notes & tracking section.  
I currently have 5 datasets I am planning on using, although some of the columns/data may not be used by the end.   
**World happiness report WHR- from https://www.kaggle.com/datasets/jainaru/world-happiness-report-2024-yearly-updated which encapsulates 2005-2024**\
**World happiness index & inflation WHI- from https://www.kaggle.com/datasets/agrafintech/world-happiness-index-and-inflation-dataset covering 2015-2023**\
**Suicide rate and life expectancy L&D- from https://www.kaggle.com/datasets/marshuu/suicide-rate-and-life-expectancy which I merged into 1 single dataset using "Country" as a key value, both from 2023**\
**Global Country Information Dataset 2023 world_data- from https://www.kaggle.com/datasets/nelgiriyewithana/countries-of-the-world-2023 from 2023**  
A last minute data source was added just to Tableau to allow "sub-regions" to be used on the dash board, as only one of the above datasets had regions and they were not friendly for sorting/using. This last dataset was added just to be able to sort by region/subregions on the Tableau dashboard.  
continents2.csv -from https://www.kaggle.com/datasets/andradaolteanu/country-mapping-iso-continent-region



## Personal notes & tracking:
Scatter plot made, based some logic on info from WHO https://www.who.int/data/gho/data/themes/topics/financial-protection  
Made 2 bar plots based on fertility rates and how happiness affects those rates.  
Made a line chart based on the bottom 20 countries, all with a happiness score under 5, showing their life expectancy of men and women.   
Made a happiness chart through the years, using input to choose a country to chart. 
Added a chart with gdp deflator index (amount of inflation), using input to choose a country to chart.  https://library.fiveable.me/key-terms/ap-macro/gdp-deflator, https://www.imf.org/en/Publications/fandd/issues/Series/Back-to-Basics/Inflation#:~:text=In%20an%20inflationary%20environment%2C%20unevenly,payers%20of%20fixed%20interest%20rates.  
Added a scatter plot of perceptions of corruption and freedom to make life choices for the 10 least happiest and most happiest countries in 2023.  
Added labels and insights and new colors to all of the charts that were completed.
Added a function to keep some code that should only run one time from erroring.  
Added functions to the charts that take input to catch input errors.
Added another chart for CO2 emissions vs forest area %. Information from markdown comes from https://www.sciencedirect.com/science/article/abs/pii/S0301479724018139  
Added another chart for infant and maternal mortality.

All data converted to SQL tables  
I used SQLiteStudio to view my tables and verify there was data in them. This was used as a troubleshooting measure when I having some issues visualizing the data and running queries on it.   
Had some issues with data being in the tables. That has been rectified and verified with a SQL query, along with the data showing in SQLiteStudio.   
Updated all tables to work properly with queries.  
Made multiple queries, looking at more things that may or may not point to what makes people happy in nations around the world.  
https://www.macrotrends.net/global-metrics/countries/wld/world/unemployment-rate   


[x] Data cleaning/organizing complete   
[x] Charts complete  
[x] SQL tables complete    
[x] SQL data wrangling complete 
[x] Completed function requirements  
[x] Completed markdown, type hinting, docstrings  
[x] Completing README requirements  
[x] Made requirements.txt  
[x] Tableau set up complete  
[x] Testing  
[ ] Finalizing/fixing/fine tuning  
