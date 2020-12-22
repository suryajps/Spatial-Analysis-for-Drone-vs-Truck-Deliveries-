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

## Plotting location of UPS Stores using  

We started with plotting 'UPS-Stores' and "UPS Customer Center Facility" on Manhattan Map. These facilities serve as access points for UPS trucks to pick-up orders that are to be delivered.

## UPS Stores and UPS Customer Center Facility in Yonkers County

<div id="folium-chart-1"></div>

## Buffer radius of 4km from each facility 

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-Yonkers-origin-Buffers.png, "20")

## Identifying 20 random samples (delivery recipients) in cluster-zone-1 

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-Yonkers-origin-destinations-Case1.png)

## Mapping one continous route from origin point (UPS facility) through the random samples (delivery recipients) and looping back to start point. 

<div id="folium-chart-2"></div>

## Identifying 20 random samples (delivery recipients) in cluster-zone-2 

![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-Yonkers-origin-destinations-Case2.png)

## Mapping one continous route from origin point (UPS facility) through the random samples (delivery recipients) and looping back to start point. 

<div id="folium-chart-3"></div>



