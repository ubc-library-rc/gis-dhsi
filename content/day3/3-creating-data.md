---
layout: default
title: Creating + editing data
nav_order: 2
parent: Tools and Workflows in QGIS
---



ALSO SHOW HOW TO CREATE AND THEN POPULATE/EDIT SHAPEFILE WITHIN QGIS. or EDIT EXISTING GEOMETRY... (could load in the canal layer or create a broken layer)


**3. Create a point over Montreal** or UdeM
Finally, we will create a point over Montreal. To do this, will use <a href="https://geojson.io/#map=2/0/20" target="_blank">geojson.io</a>, an online platform where you can click to create simple point, line, and polygon features which can then be downloaded and uploaded to a GIS. 

1. Go to <a href="https://geojson.io/#map=2/0/20" target="_blank">geojson.io</a> 

2. Simply type "Montreal" in the search bar and the webmap should zoom to the desired location. 
<img src="./images/geojson-io_20251113.png" style="width:100%">

3. Click the drop-pin icon. Your cursor should turn into a cross hair. Now click on the map, exactly where the drop-pin for Montreal is already given.     
<img src="./images/geojson-drawpoint_20251113.png" style="width:100%"> 

4. Once you click, you will notice some geoJSON code appears on the right-hand panel. This is the geoJSON that stores a single point. Click **Save** in the upper left-hand corner, and save your new point layer as either a `geojson` (notice, however, you can save as a shapefile or another file format as well). Once the file is downloaded, ***move it to your `dhsi-worshop/Day2/reference-mapping` folder. You may need to rename it to `montreal` rather than `map.geojson` which is the default. 
<img src="./images/geojson-save_20251113.png" style="width:100%">

 


Maybe also demo creating point in geojson.io??? additional info? tomorrow? yes tomorrow do a page on editing and creating shapefiles, and creating points in geojson .io 