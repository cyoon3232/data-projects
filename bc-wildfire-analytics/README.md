# Data Anlaysis: Wildfire Activity and PM2.5 in British Columbia

## 🌐 View the Rendered Project

[View the full Quarto website](https://cyoon3232.github.io/data-projects/02-build-analysis-data.html)

# About
An R and Quarto data anlaysis project.

Preventing us from opening the window during sweltering summer days is the air pollutants from fire. How much of the air pollution do wildfires actually cause? Would we be able to predict them?

This project explores the relationship between large wildfire activities and daily PM2.5 air pollutant concentration in British Columbia from 2022-2024.

It combines hourly air quality data monitored by stations from NAPS and large fire records from CNFD. 

## Project Questions

This project essentially investigated (but may not have successfully answered):

1. How did daily PM2.5 differ between 2022, 2023, and 2024? (03-eda)
2. Do stations near more recent large fires tend to experience higher PM2.5? (03-eda)
3. Can recent wildfire activity classify unusually high PM2.5 station days? (04-knn-classification)
4. Can wildfire proximity and activity predict daily mean PM2.5? (05-regression)
5. Are there distinct types of station days based on wildfire exposre and PM2.5 conditions? (06-k-means-clustering)


## Data

### Air Quality

Hourly PM2.5 observations were obtained from Environment and Climate Change Canada's National Air POllution Surveillance (NAPS) program.

Hourly observations were aggregated into a day observation. Data was valid when at least 18 hourly observations were available that day.

### Wildfires

Large-fire records were obtained from the Canadian National Fire Database (CNFD).


## Analysis Workflow

01-explore-data: explore and audit raw NAPS + wildfire data

02-build-analysis-data: hourly PM2.5 to day aggregation per station

02-build-analysis-data: wildfire date auditing

02-build-analysis-data: geographic distance calculations

02-build-analysis-data: combine air quality monitoring data and wildfire data with recent-fire features

03-eda: exploratory data analysis

04-knn-classification: KNN classification

05-regression: KNN + linear regression

06-k-means-clustering: K means clustering

07-learning-module: common mistakes turned to code-auditing module