---
layout: default
title: Georeferencing
nav_order: 4
parent: Tools and Workflows in QGIS
---
# Georeferencing Overview
{: .no_toc}

Georeferencing appends coordinate information to non-spatial data, such as images. While historical maps represent a place, tracing geographic features such as roads, rivers, buildings, cities, and political boundaries, they cannot be read by a Geographic Information System (GIS) because the locational data for these features is not stored in a manner legible to the GIS––i.e., in latitude/longitude coordinate pairs. Georeferencing is the process of warping an image so that its geographic features match the location of those on a known geospatial layer.


### Why georeference?
What do you hope to gain from georeferencing? How might georeferencing be useful in your area of research? There are many reasons one might want to georeference a historical map, included, but not limited to the following
- to render maps query-able by location or attribute data
- to add as a project basemap
- to make comparison calculations
- to serve as reference for creating shapefiles for spatial analysis or reference mapping


*Note that georeferencing is not geocoding. Geocoding is when you have a tabular dataset with street addresses and you use a GIS to geolocate the data as coordinate points.*


show me historical map where i am example
prepare to demo other options, David Rumsay Georeferencer; allmaps/IIIF; show me historical map where i am example; considerations copyright etc. pick something that doesnt have allmaps link
{: .warn}

<br>

Here are some examples of and literature on Georeferencing in the Digital Humanities
- [Don Valley Historical Map Project](https://utoronto.maps.arcgis.com/apps/webappviewer/index.html?id=6055c7fbccdf44ac911a4e13b34a825c)
- [special issue](https://www.tandfonline.com/toc/wmgl20/9/1-2) in the Journal of Map & Geography Libraries on Working Digitally with Historical Maps. 
- [Journal issue on Spatial Humanities and libraries](https://www.tandfonline.com/toc/wmgl20/19/1-2)
- [resource tutorial](https://geospatialhistorian.wordpress.com/lessons/)
- [Georeferencing in QGIS 2.0](https://programminghistorian.org/en/lessons/georeferencing-qgis)
- [georeferencing in arcgis](https://geospatialhistorian.wordpress.com/lessons/arcgis-lesson-4-digitizing/)
- [Creating New Vector Layers in QGIS 2.0](https://programminghistorian.org/en/lessons/vector-layers-qgis)
- [intro to map warper ](https://programminghistorian.org/en/lessons/introduction-map-warper)



WILL WE use map warper? IIIF? 

<details open markdown="block">
  <summary>
    On this page:
  </summary>
  {: .text-delta }
 - TOC
{:toc}
</details>

----



use 1914 and another map  - 
qgis documentation forthis workflow
have them do a newer one.... 


## Activity: Georeference a historical map with QGIS

When georeferencing within a Geographic Information System (GIS) like QGIS, the basic workflow is as follows

1. Load your Target Layer into GIS
2. Set the Coordinate Reference System (CRS) of your project
3. Load your Source Layer as a high resolution image (filetype .tif)
4. Match a handful of points on the Source Layer to those on the Target 
5. Layer, thus appending locative information to the Source Layer
6. Assess error; Adjust; Save georeferenced image


The points matched between the two layers are called **Ground Control Points (GCPs)**. When choosing a map to georeference (**Source Layer**) and geospatial reference layer(s) (**Target Layer**), it is important to ensure there are clear GCPs. GCPs may be physical geographic features, such as river bends, coastlines, or lake boundaries. GCPs may be infrastructural features such as the intersection of two roads or political boundaries or meridian lines. In any case, it is important to consider whether the geographic location of a potential GCP may have changed in the time since the historical map was rendered. These changes will matter more or less depending on the scale of the Source Layer. Most likely, your GCPs will be mix of features.



<br>

## 1. Prepare the QGIS Project



## 2. Load source data layers

- basemap? would need then a historical map relatively recent? how else to match 

## 3. Load Target Layers
We also want as a Target Layer a map of Vancouver that has street intersections since these will make excellent GCPs. We will use a plugin to connect a web-based map of the city hosted by Open Street Maps. QGIS plugins are user developed tools that extend QGIS functionality beyond the basics. To access a range of web-based maps, we’ll first install the QuickMapServices plugin. Click on the Plugin menu at the top of your screen and select Manage and Install Plugins…

In the dialogue box that opens, select All as a search category on the left and type “QuickMapServices” as one word. Install the plugin and close the dialogue box.


Now go to the Web menu at the top of your screen. You should see the QuickMapServices plugin. Hover over it and click “Settings” at the bottom of the menu that pops up. In the settings dialogue box go to the “More services” tab and click “Get contributed pack.” Click save to close settings and return to the Web menu. This time when you hover over the QuickMapServices plugin you will see an array of basemap options. Select OpenStreetMap as your basemap. Like QGIS, Open Street Map (OSM) is open source and user developed.

Make sure to drag your basemap to the bottom in your Layers Panel. Remove the basemap at anytime by right clicking the layer and selecting “remove”.


### Set Project CRS 

### CRS

do a more detailed explanation depending on whether covered in prior days


## 4. Open Georeferencer
Open the Georeferencer tool from the Layers menu at the top of your screen.

The Georeferencer window has its own toolbar. Take a minute to hover over each icon to learn what they do. The Zoom and Pan buttons work the same as those on the main QGIS interface.

## 5. Load Source Layer

###  Set Transformation Settings


## 6. Add control points





