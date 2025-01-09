---
title: "Wildfires and Air Quality in Los Angeles"
excerpt: "Wildfire and Air Quality maps for Southern California"
date: "2025-01-09"
---

<div style="font-size: 0.9em;" markdown="1">

Last updated:
{% include latest_update.txt %}

## Air Quality Map

This map shows air quality in Los Angeles based on data from outdoor PurpleAir sensors.

<div class="map-container" style="position: relative; margin: 20px 0;">
    <iframe 
        src="/assets/maps/purpleair-map.html" 
        width="100%" 
        height="600" 
        frameborder="0"
        style="border: 1px solid #ddd; border-radius: 4px;"
    ></iframe>
</div>

### What do the colors mean?

<ul style="list-style-type: none; padding-left: 20px;">

  <li><span style="color: #00e400;">●</span> <b>Good</b>: little to no risk.</li>
  <li><span style="color: #ffff00;">●</span> <b>Moderate</b>: some pollutants are present but not usually harmful.</li>
  <li><span style="color: #ff7e00;">●</span> <b>Unhealthy for Sensitive Groups</b>: people with health conditions may be affected.</li>
  <li><span style="color: #ff0000;">●</span> <b>Unhealthy</b>: everyone may start to feel effects.</li>
  <li><span style="color: #8f3f97;">●</span> <b>Very Unhealthy</b>: serious health effects may occur for everyone.</li>
  <li><span style="color: #7e0023;">●</span> <b>Hazardous</b>: emergency conditions; the entire population is more likely to be affected.</li>
</ul>

If you see many <span style="color: #ff7e00;"><b>orange</b></span>, <span style="color: #ff0000;"><b>red</b></span>, or <span style="color: #8f3f97;"><b>purple</b></span> markers, the air quality is significantly worse than usual.

## Frequently Asked Questions (FAQs)

### **How often is this updated?**

Currently, updates are done manually, but I'm working on automating the process for hourly updates soon.

### **What’s the purpose of this page?**

To make air quality information in Los Angeles more accessible and easier to understand, especially during wildfire events

### **Why should I care about air quality?**

Even if you're healthy, someone you care about might not be. Poor air quality can be dangerous for people with asthma, allergies, or heart conditions, as well as for older adults and pets.

### **Where does this data come from?**

The air quality data comes from affordable, community-installed [PurpleAir](https://www2.purpleair.com/) sensors located throughout the Los Angeles area.

### **What’s coming next?**

- Adding wildfire perimeters
- Visualizing wind direction and speed
- Integrating EPA air quality data

## Additional Information

### **What is PM2.5?**

PM2.5 refers to tiny particles in the air that are 2.5 microns or smaller. These particles can enter your lungs and bloodstream, causing health issues.

Common sources include:

- Wildfires
- Car exhaust
- Industrial emissions

### **What is AQI?**

The Air Quality Index (AQI) is a standardized scale that helps translate pollution levels into something easy to understand.

<div class="aqi-table" style="margin: 20px 0;">
    <img 
        src="/assets/img/AQI.png" 
        alt="Air Quality Index Chart" 
        style="width: 50%; max-width: 400px; display: block; margin: 0;"
    >
</div>

\*While official AQI uses 24-hour averages, this map shows recent 30-minute readings to help you stay informed about rapid changes in air quality.

## Resources

[Cal Fire](https://www.fire.ca.gov/incidents)

- Current Wildfire Emergency Incidents
- Click on an incident to view detailed maps and evacuation zones, such as the [Palisades Fire](https://www.fire.ca.gov/incidents/2025/1/7/palisades-fire)

[Watch Duty](https://www.watchduty.org/)

- Free mobile app for real-time wildfire alerts
- Available on [App Store](https://apps.apple.com/us/app/watch-duty-wildfire-maps/id1574452924), [Google play](https://play.google.com/store/apps/details?id=org.watchduty.app&pli=1) and [Web](https://app.watchduty.org/)

[AirNow](https://fire.airnow.gov/)

- Official EPA air quality visualization

[PurpleAir](https://map.purpleair.com/)

- Community-sourced air quality data

[More resources](https://www.pbssocal.org/news-community/resources-to-help-you-navigate-the-l-a-wildfires)

## Disclaimer

This page is a work in progress and should be used for informational purposes only. For official updates and health recommendations, refer to trusted sources.

</div>
