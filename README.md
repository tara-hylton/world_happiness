# world_happiness

[x] Data cleaning/organizing complete   
[x] Charts complete  
[x] SQL tables complete    
[ ] SQL data wrangling complete    
[ ] Tableau set up complete  
[ ] Testing  
[ ] Finalizing/fixing/fine tuning  

I currently have 5 datasets I am planning on using, although some of the columns/data may not be used by the end.   
world happiness report WHR- from https://www.kaggle.com/datasets/jainaru/world-happiness-report-2024-yearly-updated which encapsulates 2005-2024  
world happiness index & inflation WHI- from https://www.kaggle.com/datasets/agrafintech/world-happiness-index-and-inflation-dataset covering 2015-2023  
suicide rate and life expectancy L&D- from https://www.kaggle.com/datasets/marshuu/suicide-rate-and-life-expectancy which I merged into 1 single dataset using "Country" as a key value  
Global Country Information Dataset 2023 world_data- from https://www.kaggle.com/datasets/nelgiriyewithana/countries-of-the-world-2023 from 2023  

Scatter plot made, based some logic on info from WHO https://www.who.int/data/gho/data/themes/topics/financial-protection  
Made 2 bar plots based on fertility rates and suicide rates and how happiness affects those rates.  
Made a line chart based on the bottom 20 countries, all with a happiness score under 5, showing their life expectancy of men and women.   
Made a happiness chart through the years, using input to choose a country to look at and chart.  
Added a scatter plot of perceptions of corruption and freedom to make life choices for the least happiest and most happiest 10 countries in 2023.  
Added labels and insights to all of the charts that were completed.

Decided I needed SQL tables to continue my plot work, so have converted 2 tables to SQL so far  
All data converted to SQL tables  
I used SQLiteStudio to view my tables and verify there was data in them. This was used as a troubleshooting measure when I having some issues visualizing the data and running queries on it.   
Had some issues with data being in the tables. That has been rectified and verified with a SQL query, along with the data showing in SQLiteStudio.   
Some database names were also updated so they would not be confused with the dataframe names.  