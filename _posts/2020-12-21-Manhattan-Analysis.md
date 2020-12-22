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
There were 48 UPS customer center and UPS store facilities in the Manhattan Area, of which we assume that not all facilities would provide delivery service since they are located in close proximities. We used an unsupervised clustering algorithm to determine 3 clusters for further analysis. Each cluster has a varying number of UPS stores with figures 04, 05, and 21 UPS stores clustered for a particular label. The fourth cluster was chosen from noise samples to account for UPS Stores at farther locations.
 

![nyc-ml]({{ site.url }}{{ site.baseurl }}/assets/images/NYC_ML.png)

## Buffer radius of 1.5km from each facility: 
The urban area of Manhattan is categorized into zones (buffer radii or optimized polygon) for each UPS store. The radii for each buffer is determined to ensure minimum overlap. Each buffer zone serves as a bounding radius for the maximum travel path of trucks and drones.

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/NYC_Buffer.png)

## Origin Point and Destination Point
The origin point is located at the center of the buffer polygon. The nearest open-street-map(OSM) node is also calculated
The number of destination points in each zone are determined based on the size of the clusters and therefore the density of the neighborhood. For example, the noise cluster is assumed to have the least number of destination points while the cluster with size 24 is assumed to have most destination points.

## Delivery recipients in cluster-zones 
Selection of a number of sample points (8, 20, 35 and 45) respectively was based on the machine learning clusters. These points can always be increased incrementally.
![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/random points_nyc.png)

## Mapping Drone Paths:
Here a straight line path is plotted assuming drones would fly over the buildings to its destination point. 
![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/drones.png)
From the above analysis, total emissions for drones will be calculated based on operational carbon emissions. 

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

The calculated results can be found [here][here]



[here]:https://suryajps.github.io/Spatial-Analysis-for-Drone-vs-Truck-Deliveries-/Results-and-Conclusion/



