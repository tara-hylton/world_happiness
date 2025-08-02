# world_happiness
Jupyter notebook was used to allow for a narrative-driven presentation of code and charts.  
Pandas was used in conjuction with python to clean the data to identify what makes people happy/unhappy around the globe, along with other effects of happiness/unhappiness. All data is on a relative path.  
Matplotlib and Seaborn were used for charting purposes.  
IPython was used to clear input in areas, just to make things look nice overall.
Please run requirements.txt to download the virtual environment and all needed libraries.  

The goal of this project is to find what makes people happier in some counties versus what does not make them happy in other countries.  
The world happiness report includes: Life Ladder (happiness), Log GDP per capita, Social support, Healthy life expectancy at birth, Freedom to make life choices, Generosity, Perceptions of corruption, Positive affect, Negative affect, along with country name and year from 2005-2024, although 2023 will be mostly be used as it the common year in all of the datasets.  
The world happiness index & inflation report includes: Country, Year (2015-2023), Headline Consumer Price Inflation, Energy Consumer Price Inflation, Food Consumer Price Inflation, Official Core Consumer Price Inflation, Producer Price Inflation, GDP deflator Index growth rate, Continent/Region, Score (happiness), GDP per Capita, Social support, Healthy life expectancy at birth, Freedom to make life choices, Generosity, Perceptions of corruption.  
Suicide rate: Country, GDP per capita, Suicide rate (from 2023).  
Life expectancy: Country, Life Expectancy (years) - Men, Life Expectancy (years) - Women, Happiness Score, Fertility Rate (births per woman) (from 2023).  
Global country information dataset: Country, Density, Abbreviation, Agricultural Land( %), Land Area(Km2), Armed Forces size, Birth Rate, Calling Code, Capital/Major City, Co2-Emissions, CPI, CPI Change (%), Currency-Code, Fertility Rate, Forested Area (%), Gasoline Price, GDP, Gross primary education enrollment (%), Gross tertiary education enrollment (%), Infant mortality, Largest city, Life expectancy, Maternal mortality ratio, Minimum wage, Official language, Out of pocket health expenditure, Physicians per thousand, Population, Population: Labor force participation (%), Population: Labor force participation (%), Total tax rate, Unemployment rate, Urban_population, Latitude, Longitude.  

Statistics:  
Almost 25% of the world has low minimum wage (under 10 local) and pays over 25% of their health care costs out of pocket. (Based on amounts from the WHO, link below.)  
The 20 unhappiest countries in the world have shorter life spans, living up to 1/3 of the time of people in happier countries (expectancy 73.5). https://ourworldindata.org/grapher/life-expectancy-marimekko#:~:text=What%20you%20should%20know%20about,or%20the%20COVID%2D19%20pandemic.  
Happier countries have more freedom, or countries with more freedom are happier. Intrepret that as you will. This comes from my charts and data.

I currently have 5 datasets I am planning on using, although some of the columns/data may not be used by the end.   
world happiness report WHR- from https://www.kaggle.com/datasets/jainaru/world-happiness-report-2024-yearly-updated which encapsulates 2005-2024  
world happiness index & inflation WHI- from https://www.kaggle.com/datasets/agrafintech/world-happiness-index-and-inflation-dataset covering 2015-2023  
suicide rate and life expectancy L&D- from https://www.kaggle.com/datasets/marshuu/suicide-rate-and-life-expectancy which I merged into 1 single dataset using "Country" as a key value  
Global Country Information Dataset 2023 world_data- from https://www.kaggle.com/datasets/nelgiriyewithana/countries-of-the-world-2023 from 2023  

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
[ ] Tableau set up complete  
[ ] Testing  
[ ] Finalizing/fixing/fine tuning  
