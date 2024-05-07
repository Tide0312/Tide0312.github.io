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

## Title: Exploring Geographical Distribution of Navaids and Airports

Introduction to Dataset:

The dataset used for this analysis contains comprehensive information about navigational aids (navaids) and airports, which are crucial components of the global transportation infrastructure.

Navaids: Navaids are essential for both air and maritime navigation. They include various types of electronic devices and visual markers used by pilots and maritime navigators to determine their position, plot their course, and ensure safe navigation.
Airports: Airports are vital hubs for air travel, serving as points of departure, arrival, and transit for millions of passengers and tons of cargo every day. They provide essential facilities and services for aircraft operations, including runways, terminals, and maintenance facilities.
Dataset Description:

The dataset comprises two main components: navaids and airports. Each component includes several attributes that provide detailed information about their geographical distribution and characteristics.

Navaids Data: This dataset includes attributes such as latitude, longitude, name, type, and other relevant information about different navaids. These attributes allow us to visualize the spatial distribution of navaids and explore their diversity in terms of types and functionalities.
Airports Data: Similarly, the airports dataset contains attributes such as latitude, longitude, name, ICAO code, and other relevant details about various airports worldwide. Analyzing this data enables us to understand the global network of airports and their significance in facilitating air transportation.
Exploring the Plot:

Map of Navaids:
This map provides a visual representation of the geographical distribution of navaids around the world.
Each marker on the map represents a navaid location, with tooltips displaying additional information such as the name and type of navaid.
By exploring this map, we can gain insights into the density and coverage of navaids in different regions, which are essential for safe navigation by air and sea.

## Geographical Distribution of Navaids 

![Image]({{ site.baseurl }}/assets/pngs/heatmap.png)

{% include navaids_map-4.html %}

{% include airports_map.html %}

## Amount of Airports in Each Continent 

![Image]({{ site.baseurl }}/assets/pngs/Number_Airpots_by_Continent.png)

#### The bar chart illustrates the distribution of airports across continents. North America has the highest number of airports, almost equaling the combined total of Asia, South America, and Europe. Antarctica has the fewest airports.

## Navigation Elevations

<vegachart schema-url="{{ site.baseurl }}/assets/json/top_airports_navaids.json" style="width: 100%"></vegachart>

#### A horizontal bar chart displaying the number of navigations associated with specific airports. The bars are in descending order with the airport having the most navaids at the top. Montreal/Pierre Elliott Trudeau International Airport appears to have the highest number, around 7, while the rest have fewer, ranging from about 1 to 6.




<vegachart schema-url="{{ site.baseurl }}/assets/json/navaids_elev.json" style="width: 100%"></vegachart>

#### This histogram displays the distribution of navigations at different elevation ranges. It reveals the concentration of navaids at different altitude levels. The majority are clustered at the lower elevation ranges, indicating that most navigations are located at or near sea level.




## Number of Airports by elevation

![Image]({{ site.baseurl }}/assets/pngs/Number_of_Airports_elevation.png)

#### This bar chart, labeled "Number of Airports by Elevation Range," presents a distribution of airports according to their elevation above sea level. The most populated elevation range for airports is at 0-500 ft, with the bar peaking over 20,000 airports. The count significantly drops as elevation increases, with the 500-1,000 ft range having about half as many airports. Further increments in elevation show a steady decline in the number of airports, with those situated above 6,000 ft being exceptionally rare. This data indicates that the vast majority of airports are constructed at lower elevations, which may reflect factors such as population density, terrain, and the ease of construction and operation.

## Top Airports Runways

![Image]({{ site.baseurl }}/assets/pngs/top_airports_runways.png)

#### The chart highlights the top 10 airports with the highest number of runways. Notably, O'Hare Airport ranks first, which is quite intriguing. Among these leading airports, the majority are situated in the United States. This is consistent with the fact that North America has the densest airport network, which logically supports a busier transportation infrastructure compared to other continents.

## Runway Length and Airport Elevation by Continent

<vegachart schema-url="{{ site.baseurl }}/assets/json/runway_airport_.json" style="width: 100%"></vegachart>


#### The scatter plot compares the runway length in feet to the average airport elevation in feet across different continents, differentiated by color. Each dot represents an airport. The majority of airports, particularly in Europe and North America, are situated at lower elevations (below 2,000 feet).

## Busy Airport by Passenger in 2022

![Image]({{ site.baseurl }}/assets/pngs/top_10_busyairport.png)

<vegachart schema-url="{{ site.baseurl }}/assets/json/busy_airport.json" style="width: 100%"></vegachart>

#### Hartsfield-Jackson Atlanta International Airport is notably busier than other airports, emphasizing its role as a major hub, particularly for the United States. 
#### The clustering of total passengers around 65 million for most airports, except Atlanta, points to a competitive tier of major international airports that serve as central nodes in the global air travel network, each supporting similar volumes of traffic and potentially competing for a similar market share.

## Problems Encountered and How to Solve
#### In this project, we encountered some challenges as the person responsible for integrating our team's plots and research into Jekyll. Not all plots were in JSON format; some were tied to HTML files and couldn't be converted. We found a blog post by a Jekyll blogger explaining how to store HTML files in the 'include' folder and display HTML tables using the 'include' function. We followed these instructions successfully. However, there was an instance where this method didn't display our HTML table. After unsuccessful researches, we converted the table into a PNG file, placed it in the 'assets' folder, and successfully displayed it as a PNG on our Jekyll site.


<div class="left">
{% include elements/button.html link="https://ourairports.com/data/" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/Tide0312/Tide0312.github.io/blob/main/python_notebooks/Workbook-4.ipynb" text="The Analysis" %}
</div>
