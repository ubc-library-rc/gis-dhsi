---
layout: default
title: 1. Layer Properties
nav_order: 1
parent: Reference Mapping
---
# Modifying Layers
{: .no_toc}

Just as the QGIS Project had Project Properties, each layer has properties of its own. To view a layer's properties, right-click the layer in the Layers Panel and go to "Properties..." at the bottom. We won't dwell on all the project properties today, but notice you can learn more information about the layer here, including where it's stored on your computer, and its projection. 


<!-- 
based on [https://ubc-library-rc.github.io/gis-reference-mapping/content/hands-on3.html](https://ubc-library-rc.github.io/gis-reference-mapping/content/hands-on3.html) -->



COULD NOT PRELOAD THE CONTEXT DATA - BETTER FOR PPL TO GET A CHANCE TO UPDATE SYMBOLOGY IF ALL WERE DOING IS SOME SELECTIONS ON BAKERS. THIS WAY VISUAL HIERARCHY WOULD MAKE MORE SENSE. 

## General

## CRS
discuss. so they know. 



## Symbology
As they are, the layers we've added to our map canvas aren't particularly aesthetic, nor is foreground adequately differentiated from background. 

<!-- 
This page (and the next) will guide you through modifying your layers' symbology to create a more polished looking map where what's deemed important stands out.  -->


Symbology governs the outline and color fill of points, lines, and polygons. The symbology style for any given vector layer can be Single, Categorized, Graduated, etc. For now, let's stick with Single. This means that each layer will have a single symbology, or color/outline. 

Depending on the audience and publisher of your reference map, you might have constraints such as Black and White. Keep this in mind. For now, we'll map in color.

To Do
{: .label .label-green }
Change the color of the ocean.

1. Right-click the ocean layer and go to Properties --> Symbology. 
2. Click down to Simple Fill. 
3. Click on the color bar to change the color. Expand the dialogue window if necessary. 
4. You can also change the "stroke", or outline color, or, by setting Stroke style to "No line", remove it all together. 

[images]

 If you want to make your map in Black & White, change the Color Model from RGB to CYMK. Then set everything but K to 0. You can also color sample from the eye-dropper tab. 

[images]


### Categorized Symbology

eg each ward a different color ... 
etc. discuss
more about this when we practice thematic mapping. 



## Labelling 
Two project properties we _will_ concern ourselves with are **Labels** and **Symbology**. Labels allow you to add labels to a layer based on an attribute value. You can turn off the labels at any time by returning to a layer's properties, or by right-clicking the layer and clicking "Show Labels" again. 

To Do
{: .label .label-green }
Add ward labels based on `x`. You can customize your labels by increasing the text size, adding a buffer, or changing the label placement. 


