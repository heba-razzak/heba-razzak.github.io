---
title: "PurpleAirAPI: R Package"
excerpt: "Efficient retrieval and analysis of PurpleAir sensor data"
date: "2024-11-12"
categories:
  - R Packages
tags:
  - r
  - package-dev
  - api
---

## Project Overview

Working with environmental sensor data can be challenging, especially when tools for accessing the data are inconvenient or lack important features. While working on air quality monitoring for research projects, I found that existing tools didn’t meet my needs or those of my lab.

The PurpleAirAPI package was built with care to address real-world challenges in accessing and analyzing air quality data. Designed for both flexibility and ease of use, it bridges the gap between raw data and actionable insights, offering tools that simplify complex tasks while ensuring reliability. Here’s what makes it stand out:

- **Efficient Data Retrieval**: Smart time chunking for large data requests, respecting API limits.
- **Flexible Field Selection**: Empowers users to customize queries with access to all PurpleAir data fields.
- **Progress Tracking**: Progress updates for seamless long downloads, keeping users informed.
- **Robust Error Handling**: Clear actionable error messages, ensuring a smooth and frustration-free workflow.
- **Data Quality Assurance**: Automatically manages missing data and time zone adjustments.
- **Comprehensive Sensor Management**: Supports downloading data for multiple sensors simultaneously.
- **User-Centric Design**: Prioritizes usability with intuitive messages, thoughtful features, and clear documentation.

The result is a package that simplifies workflows, improves efficiency, and elevates the user experience—making air quality data more accessible and actionable for researchers, analysts, and environmental enthusiasts alike.

## Technical Implementation

The package interfaces with the PurpleAir API to provide two main functions:

```r
# Get sensor information
sensors <- getPurpleairSensors(
  apiReadKey = "YOUR_API_KEY",
  fields = c("latitude", "longitude", "date_created")
)

# Download historical data
history <- getSensorHistory(
  sensorIndex = sensor_ids,
  apiReadKey = "YOUR_API_KEY",
  startDate = "2024-01-01",
  endDate = "2024-01-31",
  average = 60,  # hourly averages
  fields = c("pm2.5_alt", "temperature", "humidity")
)
```

## Development Process

1. **Initial Need**: Identified gaps in existing tools during research work
2. **Design**: Focused on user experience and efficient data handling
3. **Implementation**: Built core functionality with R
4. **Testing**: Rigorous testing with real-world scenarios
5. **Documentation**: Comprehensive documentation and examples
6. **CRAN Submission**: Package prepared for CRAN distribution

## Applications

The package is particularly useful for:

- Environmental research projects
- Air quality monitoring
- Data analysis workflows
- Sensor network management

## Technical Stack

- **Language**: R
- **APIs**: PurpleAir API
- **Key Libraries**: httr, jsonlite
- **Documentation**: roxygen2
- **Testing**: testthat

## Links

- [GitHub Repository](https://github.com/heba-razzak/PurpleAirAPI)
- [CRAN Page](https://cran.rstudio.com/web/packages/PurpleAirAPI/index.html)

## Get Started

Install the package directly from CRAN:

```r
install.packages("PurpleAirAPI")
```

Or get the development version from GitHub:

```r
# install.packages("devtools")
devtools::install_github("heba-razzak/PurpleAirAPI")
```

---

Feel free to contact me for questions or collaboration opportunities.
