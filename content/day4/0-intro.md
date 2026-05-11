---
layout: default
title: Day 4
nav_order: 5
has_children: true
---
# Day 4: Web Mapping 

Today we will explore web maps (aka webmaps) and web mapping (aka webmapping). Web maps are a means of dynamically and interactively visualizing geospatial data. Today, you will learn how to create web maps in 3 different ways: 

1. **online**, through platforms such as [uMap](https://umap.openstreetmap.fr/en/) and [Google MyMaps](https://www.google.com/maps/about/mymaps/), 
2. with **coding**, powered by [Leaflet](https://leafletjs.com/), and 
3. with **QGIS**, using the [qgis2web plugin](https://plugins.qgis.org/plugins/qgis2web/).

Each of these methods of web mapping has its advantages and disadvantages which we will discuss. Moreover, while we emphasize that web mapping can be done entirely online without any coding necessary, it's useful to have a general understanding of how a web map works. To this end, we will break down the "anatomy" of a web map in a code editor in order to observe how the various components of a web map work together. By the end of the day, you will be equipped with the fundamental knowledge and skills to begin web mapping on your own. 


<br>

#### **Morning Session** 9am - 12pm
- Introduction to uMap and Google MyMaps, two online platforms for webmapping
- Hands on activity 1 - small groups assigned different datasets to map using either GoogleMy Maps or uMap 
- Webmapping with QGIS

#### **Afternoon Session** 1:30pm - 4pm
- Anatomy of a webmap
- Hands on with Leaflet - tinker with boilerplate map 
- activity could be - run selection of data in qgis -> export as geojson - then wrap as javascript and add to project. multipart vs. part be aware for points. solve using centroid. 
- hosting with github (make sure there's time for that)


<br>



## What we will make

Below are examples of webmap made with uMap, Google MyMaps, Leaflet, and QGIS.

<br>

<iframe src="./reference/leaflet-example.html" style="width:100%; height:520px; border:none;"> </iframe>
<sub>[View in Full Screen](./reference/leaflet-example.html)</sub> 


<br>


<iframe src="https://www.google.com/maps/d/embed?mid=11gHGxEF2Uxx7zbn00htegHybzWBS3ro&ehbc=2E312F&noprof=1" style="width:100%; height:520px; border:none;"></iframe>
<sub>[View in Full Screen](https://www.google.com/maps/d/embed?mid=11gHGxEF2Uxx7zbn00htegHybzWBS3ro&ehbc=2E312F&noprof=1)</sub> 

<br>

<iframe style="width: 100%; height: 520px; border: 0;" allowfullscreen src="//umap.openstreetmap.fr/en/map/toronto-public-art_1377239?scaleControl=false&miniMap=false&scrollWheelZoom=false&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#11/43.72/-79.42"></iframe>
<!-- 
<p style="font-size:11pt;"><a href="//umap.openstreetmap.fr/en/map/toronto-public-art_1377239?scaleControl=false&miniMap=false&scrollWheelZoom=true&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#11/43.72/-79.42" target="_blank">View in full screen</a></p> -->
<sub>[See full screen](//umap.openstreetmap.fr/en/map/toronto-public-art_1377239?scaleControl=false&miniMap=false&scrollWheelZoom=true&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#11/43.72/-79.42)</sub>   

<br>

<iframe src="https://lilydemet.github.io/qgis2web-example-map/" style="width:100%; height:520px; border:none;"> </iframe>
<sub>[View GitHub repo](https://github.com/lilydemet/qgis2web-example-map)</sub>   


## Before the day (or make this reminder at end of day 2)
To do - make sure you have google and umaps account. 


## Data
We will be working from the `Day3` subfolder of your `DHSI-workshop-data` folder. Inside, you will see today's data further organized into 3 subfolders relevant to webmapping online, webmapping with Leaflet, and webmapping with QGIS respectively.

We will webmap using data primarily from the [City of Toronto's open data portal](https://open.toronto.ca/catalogue/). This data is licensed under the [Open Government Licence - Toronto](https://open.toronto.ca/open-data-licence/). This allows us to modify and adapt the data! The following datasets are from the City of Toronto. They have been reformatted to be legible to the various tools and platforms we will work with today. Take a moment to browse the datasets online. 

- [Public Art](https://open.toronto.ca/dataset/public-art/)
- [Heritage Conservation Districts](https://open.toronto.ca/dataset/heritage-conservation-districts/)

<br>

- [Green Spaces](https://open.toronto.ca/dataset/green-spaces/)
- [City Wards](https://open.toronto.ca/dataset/city-wards/)
- [Regional Municipal Boundary](https://open.toronto.ca/dataset/regional-municipal-boundary/)


The QGIS Project includes province (and water features?), data from government of canada as well as - ?? from natural earth data. Data from The Government of Canada is licensced under the Open Government Licence - Canada; Data from [Natural Earth](https://www.naturalearthdata.com/) is [public domain](https://www.naturalearthdata.com/about/terms-of-use/) and therefore free to use.  



<br><br>




#### Supplementary Readings and Example DH Projects
- [Designing for discovery: using web maps in the digital humanities](https://dhq.digitalhumanities.org/vol/19/4/000819/000819.html)
- [Don Valley Historical Map Project](https://utoronto.maps.arcgis.com/apps/webappviewer/index.html?id=6055c7fbccdf44ac911a4e13b34a825c)
- [Mapping Prejudice](https://mappingprejudice.umn.edu/)
<!-- - [Queer Sapphic New York](https://zhangyuchun17.github.io/Hidden-Constellations/) -->