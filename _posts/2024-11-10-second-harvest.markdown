---
title: "Food Pantry Accessibility Analysis"
excerpt: "Interactive Tableau dashboard with geospatial insights."
categories:
  - Analytics & Visualization
tags:
  - r
  - tableau
  - dashboard
  - food bank
  - web scraping

classes: wide
date: "2024-11-10"
---

## Project Overview

An independent data analysis project examining food insecurity and pantry accessibility in Orange County. Using publicly available data, I created a comprehensive dashboard to visualize the relationship between food assistance needs and pantry availability across different regions.

## Project Goals

- Map food security resources across Orange County
- Identify gaps in pantry accessibility
- Analyze distribution of services relative to need
- Create actionable insights for resource allocation

## Interactive Dashboard

<div class='tableauPlaceholder' id='viz1732004704114' style='position: relative'>
  <noscript>
    <a href='#'>
      <img alt='Main ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Fo&#47;FoodBank_Portfolio&#47;Main&#47;1_rss.png' style='border: none' />
    </a>
  </noscript>
  <object class='tableauViz'  style='display:none;'>
    <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> 
    <param name='embed_code_version' value='3' /> 
    <param name='site_root' value='' />
    <param name='name' value='FoodBank_Portfolio&#47;Main' />
    <param name='tabs' value='no' />
    <param name='toolbar' value='yes' />
    <param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Fo&#47;FoodBank_Portfolio&#47;Main&#47;1.png' /> 
    <param name='animate_transition' value='yes' />
    <param name='display_static_image' value='yes' />
    <param name='display_spinner' value='yes' />
    <param name='display_overlay' value='yes' />
    <param name='display_count' value='yes' />
    <param name='language' value='en-US' />
  </object>
</div>
<script type='text/javascript'>
  var divElement = document.getElementById('viz1732004704114');
  var vizElement = divElement.getElementsByTagName('object')[0];
  if ( divElement.offsetWidth > 800 ) {
    vizElement.style.width='1000px';
    vizElement.style.height='827px';
  } else if ( divElement.offsetWidth > 500 ) {
    vizElement.style.width='1000px';
    vizElement.style.height='827px';
  } else {
    vizElement.style.width='100%';
    vizElement.style.height='1227px';
  }
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

[View Dashboard on Tableau Public](https://public.tableau.com/app/profile/heba.abdelrazzak/viz/FoodBankDashboard_17284458855700/Main)

## Key Metrics Analyzed

- Coverage of 256 Food Pantries and 43 TEFAP Distribution Centers
- Service to 66,784 Food-Assisted Households (6% of total households)
- 5-mile radius accessibility analysis
- Food pantry density per 1,000 food-assisted households
- Geographic distribution patterns by census tract

## Data Sources & Methodology

- U.S. Census Bureau American Community Survey (2017-2021 5-Year Estimates)
- Publicly available food pantry location data
- TEFAP distribution center information

## Technical Implementation

### Tools Used

- **Data Processing**: R for geocoding and spatial analysis
- **Visualization**: Tableau
- **Geospatial Analysis**: Census tract and block group level analysis
- **Libraries**: tidycensus, sf, dplyr

### Key Features

1. **Interactive Map View**

   - Color-coded regions showing pantry density
   - Overlay of distribution locations
   - 5-mile radius coverage analysis

2. **Accessibility Metrics**
   - Pantries per 1,000 food-assisted households
   - Block group level analysis
   - Census tract rankings

## Impact & Insights

- Identified underserved areas with high food assistance needs
- Mapped geographic disparities in resource distribution
- Created data-driven foundation for strategic planning
- Developed scalable analysis framework

## Future Enhancements

- Integration of public transportation routes
- Temporal analysis of pantry operating hours
- Demographic overlay for deeper insights
- Mobile accessibility optimization

[View Project on GitHub](https://github.com/heba-razzak/FoodBankAnalysis)
