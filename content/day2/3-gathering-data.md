---
layout: default
title: 1. Gathering Data
nav_order: 1
parent: Reference Mapping
---
# Gathering Data
{: .no_toc}

Yesterday, you learned about spatial data and where to find it. let's practice.... 





## For today's reference mapping... 
This morning we will practice making a reference map of Montreal using _vector data_ data from ???Natural Earth, Statistics Canada, and Native Land Digital.

Over top our reference map we will visualize historic bath houses. 

this data - created by Alex by... discuss. 


The workshop folder contains some of this data, as well as additional datasets for you to practice thematic mapping. However, because finding, downloading, and preparing spatial data is a major part of mapping for academic publication, you will be guided through downloading the main datasets for today's workshop on your own. Remember, move each dataset you download to the workshop folder and *unzip it* there. 


### Data needed
SWAP OUT TO MATCH WORKSHOP 
- Canadian provincial & territorial boundaries 
- World countries, lakes, and oceans
- Point over Ottawa, Canada's capital city


To Do
{: .label .label-green }    

see [here](https://ubc-library-rc.github.io/gis-reference-mapping/content/hands-on1.html)
https://ubc-library-rc.github.io/gis-reference-mapping/content/hands-on1.html

**3. Create a point over Montreal**
Finally, we will create a point over Montreal. To do this, will use <a href="https://geojson.io/#map=2/0/20" target="_blank">geojson.io</a>, an online platform where you can click to create simple point, line, and polygon features which can then be downloaded and uploaded to a GIS. 

1. Go to <a href="https://geojson.io/#map=2/0/20" target="_blank">geojson.io</a> 

2. Simply type "Montreal" in the search bar and the webmap should zoom to the desired location. 
<img src="./images/geojson-io_20251113.png" style="width:100%">

3. Click the drop-pin icon. Your cursor should turn into a cross hair. Now click on the map, exactly where the drop-pin for Montreal is already given.     
<img src="./images/geojson-drawpoint_20251113.png" style="width:100%"> 

4. Once you click, you will notice some geoJSON code appears on the right-hand panel. This is the geoJSON that stores a single point. Click **Save** in the upper left-hand corner, and save your new point layer as either a `geojson` (notice, however, you can save as a shapefile or another file format as well). Once the file is downloaded, ***move it to your `dhsi-worshop/Day2/reference-mapping` folder. You may need to rename it to `montreal` rather than `map.geojson` which is the default. 
<img src="./images/geojson-save_20251113.png" style="width:100%">

 