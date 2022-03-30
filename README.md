# Spotify-Popularity-Analysis-Song-Recommendation-Model
## Introduction
In this notebook we looked at Spotify's data and analyzed popularity of songs released from 1921 to 2020. We also built a model which recommends 10 similar songs based on one song's attributes.
## Importing models and data
We started off by importing module functions and all dependencies we need. We then uploaded our data using `pandas` and looked at the top 3 rows to get a quick overview of what our data looks like. We then used pandas' built-in `.info()` function to learn more about our data. We found that almost all of our 19 columns are either integers or floats. Four columns: `artists`,`id`,`name`, and `release_date` have a type of a object which we will change later in the notebook. The dataset contains 170,653 rows and we can also see that there is no missing values.
## Data Features Explanations
salary", "property_type", "age_days", "days_employed", "has_email", "AMT_CARD_STATUS_ENTRIES", "PCT_PAYMENTS_MISSED", "PCT_PAYMENTS_MISSED_GTR_AVG"

- **salary**: annual salary of client in dollars
- **property_type**: type of property client owns
- **age_days**: age of client in days
- **days_employed**: amount of days client has been employed (negative means they have been unemployed for the absolute value of that number. example: -46 means they have been unemployed for 46 days)
- **has_email**: does client have an email address

## Card Status Explanation
legend for "**card_status**" (make sure labels aren't encoded when viewing!):
- 0: <1 month overdue
- 1: 1-2 months overdue
- 2: 2-3 months overdue
- 3: 3-4 months overdue
- 4: 4-5 months overdue
- 5: >5 months overdue
- C: paid off that month
- X: No loan for the month

### Feature Engineered Columns
-**AMT_CARD_STATUS_ENTRIES**: how long cardholder has had credit card, in months
-**PCT_PAYMENTS_MISSED**: Using 0-5 card status and amount of card status entries
-**PCT_PAYMENTS_MISSED_GTR_AVG**: Boolean value where 1 = percent of payments missed is greater than median of percent of payments missed

## Cleaning the Data
- Renamed columns 
- Dropped occupation 
- Converted data to the proper types
- Label encoded the objects
- Used clients who have been a client for 6 months or longer

## Song Recommendation Model 

## Linear Regression Model 

### Creating Linear Regression Model Based on Best Columns Using Trained Dataframe

### Analysing Why the Model Will Not Predict Values Above 80 While Showing Actual Values up to 100

# Findings & Suggestions 
