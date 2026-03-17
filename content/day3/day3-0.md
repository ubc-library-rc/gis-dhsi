---
layout: default
title: Day 3
nav_order: 4
has_children: true
---
# Day 3: Web Mapping 

Today we will explore web maps (aka webmaps) and web mapping (aka webmapping). Web maps are dynamic, interactive maps that are hosted on the web and can be shared to others via a link. Web maps are ubiquitous in our everyday: for example, you likely use a web map on your phone to navigate around the city, track an online order, ride, or bus, and check the weather forecast near you. You will learn how to create web maps in 3 different ways: through online platforms such as uMap and Google MyMaps, through coding powered by Leaflet, and through QGIS using the qgis2web plugin.

Each of these methods of web mapping has its advantages and disadvantages which we will discuss. Moreover, while we emphasize that web mapping can be done entirely online without any coding necessary, we believe it equally important to have a basic understanding of how web maps work. To this end, we will break down the "anatomy" of a web map — the code that structures it's styling and interactivity — together in a code editor. 


<!-- Although web mapping can be done entirely online without any coding or geospatial knowledge whatsoever, it's important to understand the anatomy of a web map, that is, the various components that work together to power an interactive and dynamic map hosted on the web. For this reason, 
-->
<br>

##### **Day 3 Learning Objectives:**

1. Understand the anatomy of a web map, that is, the various components that work together to power an interactive and dynamic map hosted on the web;
2. Become familiar with the different tools and platforms available for web mapping, including the advantages and disadvantages of each; and
3. Be equipped with the fundamental knowledge and skills to begin web mapping on your own.  



<br>

#### **Morning Session** 9am - 12pm
- Introduce and Demo uMap and Google MyMaps, two online platforms for webmapping
- Hands on activity 1 - small groups assigned different datasets to map using either GoogleMy Maps or uMap 
- Anatomy of a webmap - conceptual intro to leaflet

#### **Afternoon Session** 1:30pm - 4pm
- Hands on with Leaflet - tinker with boilerplate map 
- activity could be - run selection of data in qgis -> export as geojson - then wrap as javascript and add to project. multipart vs. part be aware for points. solve using centroid. 
- qgis2plugin (webmapifying a pre-made qgis project)
- hosting with github (make sure there's time for that)




Below is an example webmap made from umap, Google MyMaps, Leaflet, and QGIS.

<iframe src="./reference/leaflet-example.html" style="width:100%; height:520px; border:none;"> </iframe>


<br>

<iframe src="https://www.google.com/maps/d/embed?mid=11gHGxEF2Uxx7zbn00htegHybzWBS3ro&hl=en&ehbc=2E312F" style="width:100%; height:520px; border:none;"></iframe>

<br>

<iframe style="width: 100%; height: 520px; border: 0;" allowfullscreen src="//umap.openstreetmap.fr/en/map/toronto-public-art_1377239?scaleControl=false&miniMap=false&scrollWheelZoom=false&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#11/43.72/-79.42"></iframe><p><a href="//umap.openstreetmap.fr/en/map/toronto-public-art_1377239?scaleControl=false&miniMap=false&scrollWheelZoom=true&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#11/43.72/-79.42" target="_blank">See full screen</a></p>


<br>

<iframe src="https://lilydemet.github.io/qgis2web-example-map/" style="width:100%; height:520px; border:none;"> </iframe>






super sub script - view github repo https://github.com/lilydemet/qgis2web-example-map



<br><br>

----

#### Resources 
- [Introduction to Webmapping with Leaflet](https://ubc-library-rc.github.io/gis-intro-leaflet/)
- [Webmapping with QGIS qgis2web](https://ubc-library-rc.github.io/gis-plugins-qgis/content/webmapping.html)
- [Hosting your webmap with GitHub Pages](https://ubc-library-rc.github.io/gis-intro-leaflet/content/hands-on9.html)







