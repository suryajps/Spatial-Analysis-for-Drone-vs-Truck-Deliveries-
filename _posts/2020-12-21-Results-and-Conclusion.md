---
title: "Results and Conclusion"
date: 2020-12-21
published: true
tags: [dataviz, matplotlib]
excerpt: "Testing package delivery in an urban-block street network" 
toc: true
toc_sticky: true
read_time: false
---

## Heatmap of kgCO2 Emission Differences 
CO2 emission calculations for truck is based on distance traveled. As carbom emission for drones cannot be accounted solely based on its miles taveled, a secnd factor, Average Energy Requirement(AER) was introduced to normalize energy expended by truck and drones for comparison. 3 sub scenarios were created with AERdrones of 30Wh/mile, 60Wh/mile and 90Wh/mile. The final Seaborn plot shows a heatmap of CO2 emission differences between drone and truck delivery conditions and varying drone energy requirement in urban (Manhattan) and sub-urban (Yonkers) area. Cells with negative values indicate that drone emit less CO2 than Trucks.  

Manhattan
![nyc-ml]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-Manhattan-Co2-Comparison.png)

Yonkers County
![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-Yonkers-Co2-comparison.png)
