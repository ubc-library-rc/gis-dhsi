---
layout: default
title: Vector Analysis Tools
nav_order: 1
parent: Tools and Workflows in QGIS
has_children: true 
---

puzzles
how many bakers (from all datasets - could run merge) are not within 5 km from a bakery? or something. idk. could do a better question that doesnt presume bakers work at nearest bakery, 

Tools and Workflows in 
intro to spatial patial analysis vector tools

clip, buffer, intersect, difference

selections: by attribution (done), location, distance

count points in polygon

change projection

JOINS and extract attribute selection - will do in reference mapping
MAYBE THIS HAD TO GO IN REFERENCE MAPPING ? JOINS ETC. 

ALSO CALCULATING AREA - THAT WOULD GO IN ATTRIBUTE TABLE SECTION - ALSO IN MORNING....

editing attribute table - calculating area

# Vector Tools
{: .no_toc}

This page will introduce some common vector tools for spatial analysis workflows. Vector tools can be accessed from the **Vector** menu, and are grouped by task: Geoprocessing, Geometry, Analysis, Research, and Data Management. You can also search for vector tools (and any other tool, for that matter) by name from the **Processing Toolbox**. The  Processing Toolbox is a panel that can be opened from **Processing** menu at the top of your screen.



If for some reason you can't find the Processing Toolbox, you may have to enable the processing plugin. In the main menu bar at the top of your screen, click on **Plugins**, then click on **Manage and Install Plugins…**. On the search bar, type in Processing. Select the Processing box and then click Close. You should now see the Toolbox icon and be able to proceed with the next steps.
{: .note}


<details open markdown="block">
  <summary>
    Vector Tools:
  </summary>
  {: .text-delta }
 - TOC
{:toc}
</details>


## Geoprocessing
Geoprocessing tools are useful for modifying the spatial extent of features, particularly in relationship to other layers. Geoprocessing is often done in the beginning of a QGIS project to prepare the data layers for further analysis. 

<img src="./images/tools1.png" style="width:100%;">


Clicking a tool will open a dialogue window specific to that tool. On the right hand side will be a description of what the tool does, and on the left, prompts for selecting input layers as well as saving the output layer to a file. 


### Clip


### Buffer


### Difference 


### Dissolve?


### Intersection?




## Geometry
The geometry tools are useful for operations to do with the geometric shape of the feature layer.

<img src="./images/tools.png" style="width:100%;">


### Centroids
Centroids will calculate the geometric center of each feature and output a layer consisting of those points. To practice, run Centroids on /// 



## Analysis
The Analysis cluster contains vector tools for performing basic statistical analysis on layers.


### Count points in polygon
Count points in polygon will add up the total features in a point layer that fall inside each feature of a polygon layer. 

### ?


## Research
The Research cluster of Vector tools –> Selections and generating random points for test scenarios.

### Select by location


### Select within Distance


### 



## Data Management 
The Data Management cluster of Vector tools is useful for modifying the data layer itself. For example, Reproject changes the data layer’s stored projection


### Merge 

### Reproject



----


# Designing Workflows
{: .no_toc}
Now it’s time to put everything you learned together by designing workflows to answer spatial questions. Using the tools above, think through how you might solve for the following…