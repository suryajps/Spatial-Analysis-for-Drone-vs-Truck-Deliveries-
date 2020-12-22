---
title: "Package Delivery using Truck and Drones in Manhattan"
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

## Plotting location of UPS Stores using  

We started with plotting 'UPS-Stores' and "UPS Customer Center Facility" on Manhattan Map. These facilities serve as access points for UPS trucks to pick-up orders that are to be delivered.

## UPS Stores and UPS Customer Center Facility in Manhattan

<div id="folium-chart-1"></div>

## Un-supervised Clustering Analysis to geo-locate proximity of facilities

![nyc-ml]({{ site.url }}{{ site.baseurl }}/assets/images/NYC_ML.png)

## Buffer radius of 1.5km from each facility 

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/NYC_Buffer.png)

## Identifying 20 random samples (delivery recipients) in cluster-zone-1 

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-NYC-Geopandas0.png)

## Mapping one continous route from origin point (UPS facility) through the random samples (delivery recipients) and looping back to start point. 

<div id="folium-chart-2"></div>

## Identifying 20 random samples (delivery recipients) in cluster-zone-1 

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-NYC-Geopandas1.png)

## Mapping one continous route from origin point (UPS facility) through the random samples (delivery recipients) and looping back to start point. 

<div id="folium-chart-3"></div>

## Identifying 20 random samples (delivery recipients) in cluster-zone-1 

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-NYC-Geopandas2.png)

## Mapping one continous route from origin point (UPS facility) through the random samples (delivery recipients) and looping back to start point. 

<div id="folium-chart-4"></div>

## Identifying 20 random samples (delivery recipients) in cluster-zone-1 

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-NYC-Geopandas3.png)

## Mapping one continous route from origin point (UPS facility) through the random samples (delivery recipients) and looping back to start point.

<div id="folium-chart-5"></div>

Below, we show the distance between residential sales and the average distance to the 5 nearest 311 calls for abandoned cars.

