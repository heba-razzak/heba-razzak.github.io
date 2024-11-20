---
title: "Air Quality Prediction"
excerpt: "Machine Learning project"
categories:
  - Machine Learning
tags:
  - r
  - xgboost
  - geospatial
date: "2024-11-01"
---

## Project Overview

- Developing machine learning models to predict air quality using diverse data sources
- Created two supporting R packages to streamline research workflow
- Processing and analyzing massive environmental and traffic datasets

### Components

1. **Air Quality Prediction Model**

   - Data cleansing and preparation
   - Exploratory data analysis
   - Geospatial operations
   - Dataset integration
   - Feature engineering
   - Processing 100M+ rows of environmental data
   - [View Project](https://github.com/heba-razzak/AirQualitySF)

2. **Custom R Packages**
   - [purpleAirAPI](https://github.com/heba-razzak/purpleAirAPI): Streamlined PurpleAir data collection
   - [DataOverviewR](https://github.com/heba-razzak/DataOverviewR): Automated EDA and reporting

### Technical Stack

- **Languages**: R
- **Key Libraries**: sf, dplyr, ggplot2, randomForest
- **Data Sources**: PurpleAir sensors, OpenStreetMap, Uber Movement, Air Quality System (US EPA), [Wildland Fire Perimeters (CalFire)](https://www.fire.ca.gov/what-we-do/fire-resource-assessment-program/fire-perimeters), Weather (Iowa Environmental Mesonet), OpenStreetMap
