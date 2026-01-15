---
layout: default
title: Georeferencing Activity
nav_order: 2
parent: Day 4
has_children: true
---
# Georeference a historical map with QGIS

Describe target and source layer


## Workflow Overview
When georeferencing within a Geographic Information System (GIS) like QGIS, the basic workflow is as follows

1. Load your Target Layer into GIS
2. Set the Coordinate Reference System (CRS) of your project
3. Load your Source Layer as a high resolution image (filetype .tif)
4. Match a handful of points on the Source Layer to those on the Target 
5. Layer, thus appending locative information to the Source Layer
6. Assess error; Adjust; Save georeferenced image


The points matched between the two layers are called **Ground Control Points (GCPs)**. When choosing a map to georeference (Source Layer) and geospatial reference layer(s) (Target Layer), it is important to ensure there are clear GCPs. GCPs may be physical geographic features, such as river bends, coastlines, or lake boundaries. GCPs may be infrastructural features such as the intersection of two roads or political boundaries or meridian lines. In any case, it is important to consider whether the geographic location of a potential GCP may have changed in the time since the historical map was rendered. These changes will matter more or less depending on the scale of the Source Layer. Most likely, your GCPs will be mix of features.