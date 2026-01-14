---
layout: default
title: EDA Analysis
---

# DEA Analysis

## Dataset Information

**Dataset:** USGS Earthquake Data (All Earthquakes, Past Month)  
**Source:** U.S. Geological Survey (USGS)  
**URL:** [https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_month.csv](https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_month.csv)  
**License:** U.S. Public Domain  
**Date Accessed:** October 23, 2025  
**Time Period:** Past 30 days

<div style="overflow-x:auto;">
    <table style="width:100%; border-collapse: collapse; font-family: sans-serif; font-size: 14px; line-height: 1.5;">
        <thead>
            <tr style="background-color: #f2f2f2; border-bottom: 2px solid #ddd; text-align: left;">
                <th style="padding: 12px; border: 1px solid #ddd;">Attribute Name</th>
                <th style="padding: 12px; border: 1px solid #ddd;">Attribute Type</th>
                <th style="padding: 12px; border: 1px solid #ddd;">Data Semantics</th>
                <th style="padding: 12px; border: 1px solid #ddd; text-align: center;">Cardinality</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">time</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Quantitative (Sequential, Temporal)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Timestamp of earthquake occurrence in ISO 8601 format</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">6,281</td>
            </tr>
            <tr style="background-color: #fafafa;">
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">latitude</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Quantitative (Sequential)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Spatial coordinate (°), range: ~–65.6 to 85.1</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">5,074</td>
            </tr>
            <tr>
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">longitude</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Quantitative (Sequential)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Spatial coordinate (°), range: ~–179.9 to 179.9</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">5,265</td>
            </tr>
            <tr style="background-color: #fafafa;">
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">depth</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Quantitative (Sequential)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Depth below Earth’s surface (km), range: approx –3.2 to 643.1</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">3,330</td>
            </tr>
            <tr>
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">mag</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Quantitative (Sequential)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Earthquake magnitude on a standard scale, range: approx –2.1 to 7.6</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">492</td>
            </tr>
            <tr style="background-color: #fafafa;">
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">magType</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Categorical (Nominal)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Type of magnitude calculation</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">7</td>
            </tr>
            <tr>
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">nst</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Quantitative (Sequential)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Number of seismic stations that recorded the event</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">146</td>
            </tr>
            <tr style="background-color: #fafafa;">
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">gap</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Quantitative (Sequential)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Largest azimuthal gap between adjacent stations (°)</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">319</td>
            </tr>
            <tr>
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">dmin</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Quantitative (Sequential)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Horizontal distance from epicenter to nearest station (°)</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">4,440</td>
            </tr>
            <tr style="background-color: #fafafa;">
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">rms</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Quantitative (Sequential)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Root-mean-square travel time residual (s)</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">159</td>
            </tr>
            <tr>
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">net</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Categorical (Nominal)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Network code of contributing organization</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">12</td>
            </tr>
            <tr style="background-color: #fafafa;">
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">id</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Categorical (Nominal)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Unique identifier for each earthquake event</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">6,281</td>
            </tr>
            <tr>
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">updated</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Quantitative (Sequential, Temporal)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Timestamp of last data update (ISO 8601)</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">6,281</td>
            </tr>
            <tr style="background-color: #fafafa;">
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">place</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Categorical (Nominal)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Human-readable text description of location</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">3,334</td>
            </tr>
            <tr>
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">type</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Categorical (Nominal)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Type of seismic event (e.g., earthquake, quarry blast, explosion)</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">3</td>
            </tr>
            <tr style="background-color: #fafafa;">
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">horizontalError</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Quantitative (Sequential)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Uncertainty estimate of horizontal position (km)</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">1,885</td>
            </tr>
            <tr>
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">depthError</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Quantitative (Sequential)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Uncertainty estimate of depth (km)</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">2,415</td>
            </tr>
            <tr style="background-color: #fafafa;">
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">magError</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Quantitative (Sequential)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Uncertainty estimate of magnitude</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">2,165</td>
            </tr>
            <tr>
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">magNst</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Quantitative (Sequential)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Number of stations used to calculate magnitude</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">208</td>
            </tr>
            <tr style="background-color: #fafafa;">
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">status</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Categorical (Ordinal)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Review status: automatic < reviewed</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">2</td>
            </tr>
            <tr>
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">locationSource</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Categorical (Nominal)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Network code for original location determined</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">12</td>
            </tr>
            <tr style="background-color: #fafafa;">
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">magSource</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Categorical (Nominal)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Network code for original magnitude determined</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">12</td>
            </tr>
            <tr>
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">mag_ordinal</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Categorical (Ordinal)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Categorized magnitude (Minor to Major)</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">5</td>
            </tr>
            <tr style="background-color: #fafafa;">
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">depth_ordinal</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Categorical (Ordinal)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Categorized depth levels</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">4</td>
            </tr>
            <tr>
                <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2c3e50;">gap_level</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Categorical (Ordinal)</td>
                <td style="padding: 10px; border: 1px solid #ddd;">Binned azimuthal gap level</td>
                <td style="padding: 10px; border: 1px solid #ddd; text-align: center;">4</td>
            </tr>
        </tbody>
    </table>
</div>

## Analysis

<iframe src="{{ site.baseurl }}/charts/mag_net_boxplot.html" class = "chart-small"></iframe>

Despite the different locations, each network has pretty similar and consistent results, with the US being the exception. Our interpretation is that the US is likely recording the most earthquakes around the world and that could contribute to more outliers. 

<iframe src="{{ site.baseurl }}/charts/net_density_chart.html" class = "chart-small"></iframe>

The graph clearly separates the goals of the seismic networks:
High-Density Regional Networks: ('ci', 'hv', 'nc', etc.) prioritize detection completeness and high resolution for small-to-micro earthquakes to study local fault mechanics. 
Broad-Scope Global Network: ('us') prioritizes breadth of coverage and the reliable recording of moderate-to-large events that pose a hazard. 

<iframe src="{{ site.baseurl }}/charts/bar_charts.html" class = "chart-square"></iframe>

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
