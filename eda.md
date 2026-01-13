---
layout: default
title: EDA Analysis
---

### DEA Analysis
<iframe src="{{ site.baseurl }}/charts/mag_net_boxplot.html" class = "chart-small"></iframe>

Despite the different locations, each network has pretty similar and consistent results, with the US being the exception. Our interpretation is that the US is likely recording the most earthquakes around the world and that could contribute to more outliers. 

<iframe src="{{ site.baseurl }}/charts/net_density_chart.html" class = "chart-small"></iframe>

The graph clearly separates the goals of the seismic networks:
High-Density Regional Networks: ('ci', 'hv', 'nc', etc.) prioritize detection completeness and high resolution for small-to-micro earthquakes to study local fault mechanics. 
Broad-Scope Global Network: ('us') prioritizes breadth of coverage and the reliable recording of moderate-to-large events that pose a hazard. 

<iframe src="{{ site.baseurl }}/charts/bar_charts.html" class = "chart-small"></iframe>

The above graphs are a collection basic bar charts of the frequency of earthquakes in relation to the respective attributes of interest. 

The chart(left) visually demonstrates that while small earthquakes occur everywhere, the most severe seismic hazard, represented by the proportion of Strong and Major quakes, is highly concentrated geographically, particularly at the extremes of the sampled latitude range (high northern and high southern latitudes), corresponding to major plate boundaries like the Circum-Pacific Belt. 

The chart(right) graphically demonstrates that the seismic hazard (the relative proportion of larger, potentially damaging quakes) is concentrated along the Pacific margins (the Ring of Fire), particularly in the Western Hemisphere longitudes, while activity elsewhere is dominated by small, non-destructive events

<iframe src="{{ site.baseurl }}/charts/spatial_map.html" class = "chart-small"></iframe>

Circum-Pacific Belt (Ring of Fire): The most striking feature is the dense clustering of earthquakes along the edges of the Pacific Ocean (roughly Longitude -180 to -70 and 100 to 180). This region is the famous "Ring of Fire," where the majority of the world's large, shallow, and deep earthquakes occur, primarily due to subduction zones. 

Absence in Continental Interiors: There are very few epicenters in the centers of major continental landmasses (e.g., central Africa, central North America, central South America, central Eurasia), confirming that most significant seismicity occurs at plate boundaries

Mid-Ocean Ridges: A scattered, linear pattern of small, shallow earthquakes is visible in the middle of the Atlantic Ocean and the southern Pacific (e.g., near Longitude -10, 0, and 100). These correspond to mid-ocean ridges (divergent boundaries), which typically produce many small, shallow quakes

<iframe src="{{ site.baseurl }}/charts/mag_depth_scatter.html" class = "chart-small"></iframe>

The overwhelming majority of the data points are clustered between 0 km and 100 km depth. The density of points drops off dramatically after 100 km. This confirms that most earthquakes, regardless of magnitude, occur in the Earth's brittle upper crust and lithosphere where rocks are cold and rigid enough to store and release elastic strain energy. This is a fundamental concept in seismology. 

<iframe src="{{ site.baseurl }}/charts/depth_density_chart.html" class = "chart-small"></iframe>

Shallow (0–70 km)
Distribution: Bimodal — a large peak at M ≈ 1.5 (many small local quakes) and a smaller peak at M ≈ 4.5 (moderate-to-large quakes).
Significance: Occur in the brittle crust, spanning the widest magnitude range (below 0 to ~7.5). Most destructive earthquakes occur here.

Intermediate (70–300 km)
Distribution: Similar to shallow quakes but dominated by small magnitudes (M ≈ 1.5) and contributing to the M ≈ 4.5 peak.
Significance: Happen within subducting slabs; capable of small to moderate magnitudes but fewer large quakes than shallow ones.

Deep (≥300 km)
Distribution: Very narrow, strongly peaked around M ≈ 4.5. No micro-quakes (M < 2), and rarely exceed M 6.
Significance: Large quakes cannot occur due to high temperature and pressure making rocks ductile.

Negative (<0 km)
Distribution: Smallest group, concentrated at M < 1.0.
Significance: Represents highly sensitive detections of micro-events, often from precise measurement methods; not true “above-surface” quakes.