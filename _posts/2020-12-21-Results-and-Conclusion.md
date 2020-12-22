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

Manhattan* <br />

![nyc-ml]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-Manhattan-Co2-Comparison.png)

Yonkers County* <br />
![nyc-buffer]({{ site.url }}{{ site.baseurl }}/assets/images/2020-12-21-Yonkers-Co2-comparison.png)

Conclusion:
•	Since the scope of analysis is limited to a 1 mile radius, the emissions of drones had negligible differences with varying energy requirements in all conditions. 
•	We could infer that a higher difference in CO2 emissions was due to larger distances (number of points in the case of urban condition) leading to trucks emitting more CO2 than drones.  
•	In order to study a scenario where drones emit more CO2, a larger radius may have to be considered and studied. 
•	We see a similar scenario in sub-urban conditions as well with truck emissions exceeding drone emissions resulting in higher differences. 
•	However, a valid comparison between urban and sub-urban condition cannot be established given that UPS stores are scarcely located, number of deliveries and times of delivery is uncertain.

