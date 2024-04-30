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

![Image]({{ site.baseurl }}/assets/pngs/heatmap.png)

{% include navaids_map-4.html %}


## Amount of Airports in Each Continent 

![Image]({{ site.baseurl }}/assets/pngs/Number_Airpots_by_Continent.png)

#### The bar chart compares the number of airports on each continent. Most of the airports are majorly located in North America, and Antarctica has the lowest.

## Navigation Elevations

<vegachart schema-url="{{ site.baseurl }}/assets/json/top_airports_navaids.json" style="width: 100%"></vegachart>

#### A horizontal bar chart displaying the number of navigations associated with specific airports. The bars are in descending order with the airport having the most navaids at the top. Montreal/Pierre Elliott Trudeau International Airport appears to have the highest number, around 7, while the rest have fewer, ranging from about 1 to 6.




<vegachart schema-url="{{ site.baseurl }}/assets/json/navaids_elev.json" style="width: 100%"></vegachart>

#### This histogram displays the distribution of navigations at different elevation ranges. It reveals the concentration of navaids at different altitude levels. The majority are clustered at the lower elevation ranges, indicating that most navigations are located at or near sea level.




## Number of Airports by elevation

![Image]({{ site.baseurl }}/assets/pngs/Number_of_Airports_elevation.png)


## Top Airports Runways

![Image]({{ site.baseurl }}/assets/pngs/top_airports_runways.png)

## Runway Length and Airport Elevation by Continent

<vegachart schema-url="{{ site.baseurl }}/assets/json/runway_airport_.json" style="width: 100%"></vegachart>


#### The scatter plot compares the runway length in feet to the average airport elevation in feet across different continents, differentiated by color. Each dot represents an airport. The majority of airports, particularly in Europe and North America, are situated at lower elevations (below 2,000 feet).

## Problems Encountered and How to Solve