# Folium Visual Analytics: SpaceX Falcon 9 First Stage Landing

## Overview
The success rate on a launch may depend on its launch site. The locations of previous launch sites were analyzed to discover aspects that could help determine optimal launch conditions.

## Data Visualization Objectives

### Marking All Launch Sites
A folium map was implemented on an aggregated dataset of the launch sites. The average latitude and longitude coordinates were used to plot each launch site, which can be shown in the following map:

![Launch Site Locations](https://github.com/Cameron-Nann-Python/ibm_data_science_capstone_rocket_launch_prediction/blob/main/step_5_visual_analytics_folium/maps/launch_sites.html)

It was observed all previous launch sites were situated near coastlines. 

### Marking All Successful and Unsuccessful Launches
A MarkerCluster group was added to the map to group each launch with it's outcome. Successful launches were designated with a green marker and unsuccessful launches were designated with a red marker. The map appears as follows:

![Launch Site Outcomes](https://github.com/Cameron-Nann-Python/ibm_data_science_capstone_rocket_launch_prediction/blob/main/step_5_visual_analytics_folium/maps/outcome_sites.html)

### Calculate Distance between Launch Site and Proximities
The distance between the launch site and nearby locations, a coastline and a highway, were observed. From the VAFB SLC-4E launch site, the closest coastline was 1.36 km away:

![Closest Coastline](https://github.com/Cameron-Nann-Python/ibm_data_science_capstone_rocket_launch_prediction/blob/main/step_5_visual_analytics_folium/screenshots/closest_coastline.png)

From the KSC LC-39A launch site, the closest highway was 0.83 km away:
![Closest Highway](https://github.com/Cameron-Nann-Python/ibm_data_science_capstone_rocket_launch_prediction/blob/main/step_5_visual_analytics_folium/screenshots/closest_highway.png)

## Considerations
The optimal launch site location parameters include:
- access to a coastline
- access to a railroad
- access to a highway
- far away from nearby cities

## Technnologies Use
- Python 3.13
- Folium
- Pandas

## Import Libraries
Run the following code in a virtual environment:
```
pip install -r requirements.txt
```

## Files Included 
- `lab_jupyter_launch_site_location.ipynb`: Lab notebook on visual analysis provided by IBM
- maps folders: html maps of launch sites
- screenshots: .png files of distance measurements
