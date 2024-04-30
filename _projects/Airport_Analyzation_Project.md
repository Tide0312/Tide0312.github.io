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

## Amount of Airports in Each Continent 

![Image]({{ site.baseurl }}/assets/pngs/Number_Airpots_by_Continent.png)

## Navigation Elevations

<vegachart schema-url="{{ site.baseurl }}/assets/json/navaids_elev.json" style="width: 100%"></vegachart>


<vegachart schema-url="{{ site.baseurl }}/assets/json/top_airports_navaids.json" style="width: 100%"></vegachart>

## Number of Airports by elevation

![Image]({{ site.baseurl }}/assets/pngs/Number_of_Airports_elevation.png)


## Top Airports Runways

![Image]({{ site.baseurl }}/assets/pngs/top_airports_runways.png)

## Runway Length and Airport Elevation by Continent
<vegachart schema-url="{{ site.baseurl }}/assets/json/runway_airport.json" style="width: 100%"></vegachart>

some random stuff
{% include Number_of_Airports_by_Elevation.html %}
