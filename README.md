# Pyspark ETL Pipeline 
### Data Engineering Capstone Project
### See total description in the Pyspark-ETL-Pipeline.ipynb



#### Project Summary
This project builds an ETL pipeline for Immigration Data and City Temperature Data to form a final fact table to help answer questions on the relationships between the two datasets.

The project follows the follow steps:
* Step 1: Scope the Project and Gather Data
* Step 2: Explore and Assess the Data
* Step 3: Define the Data Model
* Step 4: Run ETL to Model the Data
* Step 5: Complete Project Write Up

### Step 1: Scope the Project and Gather Data

#### Scope 

This project consumes and aggregates I94 Immigration Data from the US National Tourism and Trade Office and Temperature Data from Kaggle to determine if there is a correlation between immigration patterns and temperature averages in cities. The data creates a fact table by joining on city. Spark is used in this process. 

#### Describe and Gather Data 
When exploring data there are several factors you have to figure out about your data before combining, cleaning, and filtering it. Below are what columns are important in each of the datasets imported.

#### Immigration Data: Us National Tourism and Trade Office (SAS7BDAT format)
I94 Immigration Data: This data comes from the US National Tourism and Trade Office. A data dictionary is included in the workspace. This is where the data comes from. There's a sample file so you can take a look at the data in csv format before reading it all in. You do not have to use the entire dataset, just use what you need to accomplish the goal you set at the beginning of the project.

* cicid = city id
* i94yr = 4 digit year
* i94mon = numeric month
* i94cit = 3 digit code of origin city
* i94port = 3 character code of destination USA city
* arrdate = arrival date in the USA
* i94mode = 1 digit travel code
* depdate = departure date from the USA
* i94visa = reason for immigration

#### Temperature data: Kaggle (csv format)
World Temperature Data: This dataset came from Kaggle. You can read more about it here.

* AverageTemperature = average temperature
* AverageTemperatureUncertainy = average temperature uncertainty
* City = city name
* Country = country name
* Latitude= latitude
* Longitude = longitude

#### Correct SAS Label Data
* i94port = numerical value
* city = city name