---
layout: default
title: Data Wrangling
nav_order: 4
parent: Day 1
---
# Data Wrangling
{: .no_toc}

or call it Data preparation - im still developing the below so feel free to contribute thoughts/text/resources
{: .warn}

Demo some management and prep practices - then give structured work time for those who want to use their data for reference mapping to make sure its prepared. includes format as well as spatial componants properly organized into separate columns. ...

get a sense of ppls data formats from survey results 
{: .warn}



<details open markdown="block">
  <summary>
    On this page:
  </summary>
  {: .text-delta }
 - TOC
{:toc}
</details>
----

<!-- 3. Creating and editing spatial data (shapefiles, geojson.io; csv prep; geolocating); and -->

## Creating a set of points/lines/polygons freehand with geojson.io 
[short description of possible scenearios in which you'd have to do this - pull from responses]
Handy tool - [geojson.io](https://geojson.io/next/) - what it does - now that you know geojson data ---

 not only is Geojson.io an easy way to create a small set of point, line, or polygon data, it is also a great tool to quickly change between formats once your data is spatialized. 


create point/polygon/line in [geojson.io](https://geojson.io/next/)


**3. Create a point over UdeM** 
Finally, we will create a point over Montreal. To do this, will use <a href="https://geojson.io/next/" target="_blank">geojson.io</a>, an online platform where you can click to create simple point, line, and polygon features which can then be downloaded and uploaded to a GIS. 

1. Go to <a href="https://geojson.io/next/" target="_blank">geojson.io</a> 
<img src="./images/geojson1.png" style="width:100%">

<br>

2. You can adjust the Basemap from the top right-hand corner.
<img src="./images/geojson2.png" style="width:100%">

3. Now, you can add points/lines/polygons either by searching places up, or zooming to known areas and simply tracing on top of the map. 

> * Let's firs try adding a point over UdeM by searching it up. Simply type "Universite de Montreal" or "University of Montreal" in the search bar and the webmap should zoom to the desired location.

<img src="./images/geojson3.png" style="width:100%">

> * Now click on the blue "Add to Map" button

<img src="./images/geojson4.png" style="width:100%">

You'll see now a point has been added to the map. Not only that, the geojson for the point is visible in the right-hand panel, and an editable table for the point data has been added to the bottom of your window.

<img src="./images/geojson5.png" style="width:100%">

4. You can also create a dataset of *either* points *or* lines *or* polygons by drawing directly onto the map. 

<img src="./images/geojson6.png" style="width:100%">

5. When you're done, you can export your geojson as geojson or shapefile or csv or kml. as you'll learn throughout the course, different platforms prefer — or even require — differently formatted data. not only is Geojson.io an easy way to create a small set of point, line, or polygon data, it is also a great tool to quickly change between formats once your data is spatialized. 

<img src="./images/geojson7.png" style="width:100%">


<br>

> other uses -> drag in csv - edit etc. need to check this out for myself
- show how you can load in data and modify etc. 



<br>

## Preparing spreadsheet data....

example - you have a csv with locations but cities or provinces or addresses, not coordinate points.. a couple options. 1 - do by hand... 

spreadsheet  data - alex will have gone over the day before adding CSV data, and considerations. 

copy paste from google maps etc.

but remember - coordintes base don projection... 




<br>

## Geocoding
Geocoding is a process by which addresses are given coordinate locations, thus allowing them to be manipulated in a GIS. In other words, geocoding transforms tabular data into spatial data. Reverse Geocoding is when you begin with a set of geolocated points (coordinates) and use a tool to get the street addresses of each point. 


### Geocoding demo 
geocoding -- use baths csv - online geocoder with addresses? see how points match. or, have other csv prepared in folder that doesnt have lat long - see how well add in and overlay existing one. 
> different to georeferencing which we'll cover at length in day 3... 
> also - note interoperability and also some platforms require certain types of data



You can geocode with QGIS.. see [here](https://ubc-library-rc.github.io/gis-plugins-qgis/content/geocoding.html) and [here](https://guides.library.ucsc.edu/DS/Resources/QGIS) to geocode with  See another [GeoCoding](https://plugins.qgis.org/plugins/GeoCoding/), another plugin specific to finding addresses or reverse geocoding. 

You don't need to geocode in a GIS! If you aren't using a GIS for any other portion of your project, consider using an online geocoder like [BC Address Geocoder](https://www2.gov.bc.ca/gov/content/data/geographic-data-services/location-services/geocoder) or [geocodio](https://www.geocod.io/free-geocoding/), or explore more free and paid options [here](https://gisgeography.com/geocoders/)


other online tools you know of/recommend? otherwise this is fine
{: .warn}



<br>

## Data collection tools
- [Terrastories](https://terrastories.app/), a tool by [Awana Digital](https://awana.digital/mapeo), is a great resource for collecting place-based data on the go.
- [ArcGIS Survey 124](https://survey123.arcgis.com/) allows you to collect surveys with spatial information. 

more? phone apps?
{: .warn}
