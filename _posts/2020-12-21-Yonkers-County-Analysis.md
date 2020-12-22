---
title: "Yonkers County Analysis"
date: 2020-12-21
published: true
tags: [dataviz, matplotlib]
excerpt: "Testing package delivery in an urban-block street network"
folium-loader:
  folium-chart-1: ["/assets/Yonkers_Images/Folium/2020-12-21-Yonkers-allfacility.html", "400"] # second argument is the height
  folium-chart-2: ["/assets/Yonkers_Images/Folium/2020-12-21-Yonkers-route-case1.html", "400"] # second argument is the height
  folium-chart-3: ["/assets/Yonkers_Images/Folium/2020-12-21-Yonkers-route-case2.html", "400"] # second argument is the height


toc: true
toc_sticky: true
read_time: false
---

## Package Delivery using Truck and Drones in Yonkers County

## Plotting UPS Store Locations
We started with plotting 'UPS-Stores' and "UPS Customer Center Facility" on Manhattan Map. These facilities serve as access points for UPS trucks to pick-up orders that are to be delivered.

## UPS Stores and UPS Customer Center Facility in Yonkers County
<div id="folium-chart-1"></div>

## Buffer radius of 4km from each facility: 
The suburban area of Yonkers County is categorized into zones (buffer radii or optimized polygon) for each UPS store. The radii for each buffer is determined to ensure minimum overlap. Each buffer zone serves as a bounding radius for the maximum travel path of trucks and drones.
![Yonkers-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-Yonkers-origin-Buffers.png)

## Origin Point and Destination Point
The origin point is located at the center of the buffer polygon. The nearest open-street-map(OSM) node is also calculated
The number of destination points in each zone are determined based on the size of the clusters and therefore the density of the neighborhood. For example, the noise cluster is assumed to have the least number of destination points while the cluster with size 24 is assumed to have most destination points.

## Mapping Drone Paths:
Here a straight line path is plotted assuming drones would fly over the buildings to its destination point. 
![random-points-yonkers]({{ site.url }}{{ site.baseurl }}/assets/images/random points_yonkers.png)
From the above analysis, total emissions for drones will be calculated based on operational carbon emissions.

## Mapping UPS Truck Paths:

Cluster-zone-01: 
Mapping one continous route from origin point (UPS facility) through the random samples (delivery recipients) and looping back to start point. 
<div id="folium-chart-2"></div>

Cluster-zone-02: 
Mapping one continous route from origin point (UPS facility) through the random samples (delivery recipients) and looping back to start point. 
<div id="folium-chart-3"></div>

The calculated results can be found [here][here]



[here]:https://suryajps.github.io/Spatial-Analysis-for-Drone-vs-Truck-Deliveries-/Results-and-Conclusion/



