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
Github was used for version control.  
Tableau was used for a finished product view of the project.  
Please run requirements.txt to download the virtual environment and all needed libraries.  

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
Countries:  
w_h_data: 165  
inf_data: 150  
life_death_data: 148  
gci_data: 155
Average of 154 countries used
Time: over 20 years but focused on 2023


## Data dictionary:

**World happiness index & inflation**
inf_data
country                         text  
year                            integer  
energy_inflation                float  
food_inflation                  float  
gdp_deflator_index              float  
score                           float  
gdp_per_capita                  float  
freedom_to_make_life_choices    float  

**Suicide rate and life expectancy**
life_death_data  
country                   text  
male_life_expectancy      float  
female_life_expectancy    float  
happiness_score           float  
fertility_rate            float  
gdp_per_capita            float  
suicide_rate              float  

**World happiness report**
w_h_data  
country_name                        text  
year                                integer  
happiness_score (aka life ladder)   float  
gdp_per_capita                      float  
social_support                      float  
healthy_life_expectancy_at_birth    float  
freedom_of_choice                   float  
generosity                          float  
perceptions_of_corruption           float  

**Global Country Information Dataset 2023**
gci_data  
country                             text  
density                             float  
birth_rate                          float  
co2_emissions                       float  
fertility_rate                      float  
forested_area                       float  
gdp                                 float  
primary_education_enrollment        float  
tertiary_education_enrollment       float  
infant_mortality                    float  
life_expectancy                     float  
maternal_mortality_ratio            float  
minimum_wage                        float  
out_of_pocket_health_expenditure    float  
physicians_per_thousand             float  
population                          float  
labor_force_participation           float  
tax_revenue                         float  
unemployment_rate                   float  

**continents2**  
(This was only used for Tableau as it was added last minute.)  
name (country)                      text  
region                              text  
sub-region                          text  

## Data sources:
All data sources used during this project are listed below.  Any additional information that I used while researching this project is listed in the personal notes & tracking section.  
I currently have 5 datasets I am planning on using, although some of the columns/data may not be used by the end.   
**World happiness report WHR- from https://www.kaggle.com/datasets/jainaru/world-happiness-report-2024-yearly-updated which encapsulates 2005-2024**\
**World happiness index & inflation WHI- from https://www.kaggle.com/datasets/agrafintech/world-happiness-index-and-inflation-dataset covering 2015-2023**\
**Suicide rate and life expectancy L&D- from https://www.kaggle.com/datasets/marshuu/suicide-rate-and-life-expectancy which I merged into 1 single dataset using "Country" as a key value, both from 2023**\
**Global Country Information Dataset 2023 world_data- from https://www.kaggle.com/datasets/nelgiriyewithana/countries-of-the-world-2023 from 2023**  
A last minute data source was added just to Tableau to allow "sub-regions" to be used on the dash board, as only one of the above datasets had regions and they were not friendly for sorting/using. This last dataset was added just to be able to sort by region/subregions on the Tableau dashboard.  
**continents2.csv -from https://www.kaggle.com/datasets/andradaolteanu/country-mapping-iso-continent-region**



