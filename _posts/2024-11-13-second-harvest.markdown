---
title: "Food Pantry Accessibility Analysis"
excerpt: "Tableau dashboard with geospatial insights."
categories:
  - Analytics & Visualization
tags:
  - r
  - tableau
  - dashboard
  - food bank
  - web scraping
toc: true
date: "2024-11-13"
---

## Purpose

This dashboard helps decision-makers identify **optimal locations for new food pantries** by evaluating both **need** and **accessibility** at a 5-mile radius level.

## How to Use This Dashboard

- **Find low-access areas** → **Red/orange** areas have the worst availability.
- **Check household volume** → Prioritize locations with **50+ food-assisted households**.
- **Select priority areas** → **Click and drag** on the scatter plot to **filter census tracts** on the map and bar chart.

## Interactive Dashboard

<div class='tableauPlaceholder' id='viz1732004704114' style='position: relative;'>
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
  vizElement.style.width='1000px';
  vizElement.style.height='1000px';
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

[View Dashboard on Tableau Public](https://public.tableau.com/app/profile/heba.abdelrazzak/viz/FoodBankDashboard_17284458855700/Main)

## Key Insights & Impact

- 464 households identified with no local pantry access.
- Located strategic sites where a new pantry could serve 3,000+ households.
- Mapped food insecurity gaps to help optimize food bank operations.

## The Metric Behind the Color Coding

$$
\frac{\text{Number of Food Pantries*}}{\text{Households Receiving Food Assistance* / 1000}}
\qquad\qquad \tag*{* within 5 Miles}
$$

### Why This Metric?

This metric helps **identify food pantry gaps** more effectively than using raw numbers alone:

- **5-mile radius** → Ensures fair comparisons since census tracts vary widely in size.
- **Dividing by 1,000** → Standardizes the ratio for easier interpretation.
- **Balancing need and access** → Highlights **distribution gaps** by factoring in both pantry availability and the number of food-assisted households.

## Technical Approach

This project integrates **geospatial analysis, census data, and web scraping** to identify underserved areas.

### Tools Used

- **R 4.3.2** (`tidycensus`, `sf`, `dplyr`, `ggplot2`, `stringr`) → For data processing & geospatial analysis.
- **Tableau Public** → For interactive visualization.

### Data Sources

- **Food Pantry Locations** → Web-scraped from [Second Harvest of Orange County](https://feedoc.org/need-food/).
- **Census Data** → U.S. Census Bureau (ACS 2017-2021 5-Year Estimates), accessed via R.

[View Project on GitHub](https://github.com/heba-razzak/FoodBankAnalysis)

<!-- ## Project Overview

An independent data analysis project examining food insecurity and pantry accessibility in Orange County. Using publicly available data, I created a comprehensive dashboard to visualize the relationship between food assistance needs and pantry availability across different regions.

## Project Goals

- Map food security resources across Orange County
- Identify gaps in pantry accessibility
- Analyze distribution of services relative to need
- Create actionable insights for resource allocation

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

[View Project on GitHub](https://github.com/heba-razzak/FoodBankAnalysis) -->
