---
layout: default
title: Vector Analysis Tools
nav_order: 2
parent: Tools and Workflows in QGIS
has_children: true 
---
# Vector Tools
{: .no_toc}

This page will introduce some common **vector tools** for spatial analysis workflows. As you saw yesterday, vector tools can be searched for in the **Processing Toolbox**. They can also be accessed from the **Vector menu** at the top of your screen, and are grouped by task: Geoprocessing, Geometry, Analysis, Research, and Data Management.
<!-- The Processing Toolbox is a panel that can be opened from Processing menu at the top of your screen. -->

In what follows -  introduce common vector tools in QGIS, particularly those relevant to (reference) mapping. we will return to reference mapping data and qgis project - see how some tools come in handy for analyzing, modifying, and visualizing spatial data. 


<details open markdown="block">
  <summary>
    On this page:
  </summary>
  {: .text-delta }
 - TOC
{:toc}
</details>
----


## Geoprocessing
Geoprocessing tools are useful for modifying the spatial extent of features, particularly in relationship to other layers. Geoprocessing is often done in the beginning of a QGIS project to prepare the data layers for further analysis. 

<img src="./images/tools1.png" style="width:100%;">


Clicking a tool will open a dialogue window specific to that tool. On the right hand side will be a description of what the tool does, and on the left, prompts for selecting input layers as well as saving the output layer to a file. 


### Clip
clip - provinces??? 2 mtl - this doesnt relaly do anything




### Buffer
buffer - buffer baths - show dissolve and not dissolve


### Difference 
need to have done merge here already? 
difference - parks - merged water features, so water can go below land thus show land outline
or can just do the jour


### Dissolve
dissolve - mtl


### Intersection?
intersection - - similar to join??? 


### Union??
similar to merge? 

<br>

## Data Management
management: merge vector layers; join attributes by location; reproject

The Data Management cluster of Vector tools is useful for modifying the data layer itself. For example, Reproject changes the data layer’s stored projection


### Merge 

Merge - water features

differentiate merge, dissolve, union

<!-- ## Geometry
The geometry tools are useful for operations to do with the geometric shape of the feature layer.

<img src="./images/tools.png" style="width:100%;"> 


### Centroids
Centroids will calculate the geometric center of each feature and output a layer consisting of those points. To practice, run Centroids on /// 
-->

<!-- 
## Analysis
The Analysis cluster contains vector tools for performing basic statistical analysis on layers.


### Count points in polygon
Count points in polygon will add up the total features in a point layer that fall inside each feature of a polygon layer. 

### ? -->

## Research
The Research cluster of Vector tools –> Selections and generating random points for test scenarios.

### Select by location


### Select within Distance












## Designing Workflows

Now it’s time to put everything you learned together by designing workflows to answer spatial questions. Using the tools above, think through how you might solve for the following…


----
spatial join - 
select within  -- bath in ward/neighborhood (not dissolved)
select by location - 


missed - calculate area (parks, eg) - did whole thing in thematic mapping about attribute table - check its not too much - otherwise could do that here. but still too much. just too much content all around. 


----