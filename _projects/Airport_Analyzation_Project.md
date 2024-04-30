---
name: Airport Analyzation Project
tools: [Python, HTML, vega-lite]
description: This is our "observatory". 
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Airport Analyzation Project

by Renault Kang, Spencer Lin, Jaclyn Lo, and Jas Chetan Mehta.

## Geographical Distribution of Navaids 

## Geographical Distribution of Airports

## Amount of airports in each continent 

## Navigation Elevations
<vegachart schema-url="{{ site.baseurl }}/assets/json/navaids_elev.json" style="width: 100%"></vegachart>


<vegachart schema-url="{{ site.baseurl }}/assets/json/top_airports_navaids.json" style="width: 100%"></vegachart>

## Number of Airports by elevation

{% include Number_of_Airports_by_Elevation.html %}

## Runways with airports

![Image]({{ site.baseurl }}/assets/pngs/cars.png)

## Correlation between Runway Length and Airport Elevation