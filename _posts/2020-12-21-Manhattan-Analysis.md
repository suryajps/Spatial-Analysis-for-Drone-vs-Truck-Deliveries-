---
title: "Package Delivery using Truck and Drones in Manhattan"
date: 2020-12-21
published: true
tags: [dataviz, matplotlib]
excerpt: "Testing package delivery in an urban-block street network"
folium-loader:
  folium-chart-1: ["/assets/Manhattan_Images/Folium/2020-12-21-NYC-allfacility.html", "400"] # second argument is the height
  folium-chart-2: ["/assets/Manhattan_Images/Folium/2020-12-21-NYCRoute-Folium8.html", "200"] # second argument is the height
  folium-chart-3: ["/assets/Manhattan_Images/Folium/2020-12-21-NYC-Route-Folium20.html", "400"] # second argument is the height
  folium-chart-4: ["/assets/Manhattan_Images/Folium/2020-12-21-NY-CRoute-Folium35.html", "200"] # second argument is the height
  folium-chart-5: ["/assets/Manhattan_Images/Folium/2020-12-21-NY-CRoute-Folium45.html", "200"] # second argument is the height
  

toc: true
toc_sticky: true
read_time: false
---

# Plotting location of UPS Stores

Plotting 'UPS-Stores' and "UPS Customer Center Facility" on the map of Manhattan. These facilities act as access points for UPS trucks to pick-up orders to be delivered.

## UPS Stores and UPS Customer Center Facility in Manhattan

<div id="folium-chart-1"></div>

## Un-supervised Clustering Analysis to geo-locate proximity of facilities

![nyc-ml]({{ site.url }}{{ site.baseurl }}/assets/images/NYC_ML.png)

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/NYC_Buffer.png)

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-NYC-Geopandas0.png)

<div id="folium-chart-2"></div>

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-NYC-Geopandas1.png)

<div id="folium-chart-3"></div>

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-NYC-Geopandas2.png)

<div id="folium-chart-4"></div>

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-NYC-Geopandas3.png)

<div id="folium-chart-5"></div>

Below, we show the distance between residential sales and the average distance to the 5 nearest 311 calls for abandoned cars.

