---
layout: default
title: 1. Prepare Project
nav_order: 1
parent: Georeferencing Activity
---


## Open the QGIS Project


## Load source data layers

## Load Target Layers
We also want as a Target Layer a map of Vancouver that has street intersections since these will make excellent GCPs. We will use a plugin to connect a web-based map of the city hosted by Open Street Maps. QGIS plugins are user developed tools that extend QGIS functionality beyond the basics. To access a range of web-based maps, we’ll first install the QuickMapServices plugin. Click on the Plugin menu at the top of your screen and select Manage and Install Plugins…

In the dialogue box that opens, select All as a search category on the left and type “QuickMapServices” as one word. Install the plugin and close the dialogue box.


Now go to the Web menu at the top of your screen. You should see the QuickMapServices plugin. Hover over it and click “Settings” at the bottom of the menu that pops up. In the settings dialogue box go to the “More services” tab and click “Get contributed pack.” Click save to close settings and return to the Web menu. This time when you hover over the QuickMapServices plugin you will see an array of basemap options. Select OpenStreetMap as your basemap. Like QGIS, Open Street Map (OSM) is open source and user developed.

Make sure to drag your basemap to the bottom in your Layers Panel. Remove the basemap at anytime by right clicking the layer and selecting “remove”.


## Set Project CRS 

### CRS

do a more detailed explanation depending on whether covered in prior days

