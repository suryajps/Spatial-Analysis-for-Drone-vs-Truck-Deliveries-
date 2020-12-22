---
title: "Manhattan Analysis"
date: 2020-12-21
published: true
tags: [dataviz, matplotlib]
excerpt: "Testing package delivery in an urban-block street network"
folium-loader:
  folium-chart-1: ["/assets/Manhattan_Images/Folium/2020-12-21-NYC-allfacility.html", "400"] # second argument is the height
  folium-chart-2: ["/assets/Manhattan_Images/Folium/2020-12-21-NYCRoute-Folium8.html", "400"] # second argument is the height
  folium-chart-3: ["/assets/Manhattan_Images/Folium/2020-12-21-NYC-Route-Folium20.html", "400"] # second argument is the height
  folium-chart-4: ["/assets/Manhattan_Images/Folium/2020-12-21-NYC-Route-Folium35.html", "400"] # second argument is the height
  folium-chart-5: ["/assets/Manhattan_Images/Folium/2020-12-21-NYC-Route-Folium45.html", "400"] # second argument is the height
  

toc: true
toc_sticky: true
read_time: false
---
## Package Delivery using Truck and Drones in Manhattan
## Plotting UPS Store Locations

We started with plotting 'UPS-Stores' and "UPS Customer Center Facility" on Manhattan Map. These facilities serve as access points for UPS trucks to pick-up orders that are to be delivered.

## UPS Stores and UPS Customer Center Facilities in Manhattan

<div id="folium-chart-1"></div>

## Un-supervised Clustering Analysis to geo-locate proximity of facilities
There were 48 UPS customer center and UPS store facilities in the Manhattan Area, of which we assume that not all facilities would provide delivery service since they are located in close proximities. Hence, we.... 

![nyc-ml]({{ site.url }}{{ site.baseurl }}/assets/images/NYC_ML.png)

## Buffer radius of 1.5km from each facility: 

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/NYC_Buffer.png)

## Mapping Drone Paths:
Here a straight line path is plotted assuming drones would fly over the buildings to its destination point. 

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/drones.png)


## Identifying 8, 20, 35 and 45 random samples (delivery recipients) in cluster-zones 
Selection of number of sample points was based on ....

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/random points_nyc.png)

## Mapping Truck Paths:
Mapping one continous route from origin point (UPS facility) through the random samples (delivery recipients) and looping back to start point. 

Truck path for 8 delivery locations
<div id="folium-chart-2"></div>

Truck path for 20 delivery locations
<div id="folium-chart-3"></div>

Truck path for 35 delivery locations
<div id="folium-chart-4"></div>

Truck path for 45 delivery locations
<div id="folium-chart-5"></div>

From the above analysis, we calculated the Vehicle Miles Traveled and associated CO2 Emissions for Trucks.



