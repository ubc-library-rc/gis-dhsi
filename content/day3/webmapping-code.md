---
layout: default
title: Webmapping with Code
nav_order: 3
parent: Day 3
---
# Webmapping with Code


<img src="./images/leaflet-logo.png" alt="Leaflet Logo" style="margin: auto; width:35%"/>

[Leaflet](https://leafletjs.com/) is a set of instructions that your web browser or mobile device uses to display maps and let you interact with them. For example, when you double click your mouse on a map, leaflet tells your browser to zoom in. Leaflet defines the style of your map and includes things like zoom controls, attribution links, pop-ups, colors for markers and more. Leaflet is made up of only 38kb of Javascript, so it is really fast and lightweight - meaning browsers don’t have to work very hard to load it. Leaflet is open source, free, and hugely customizable. And, because of this, Leaflet is widely used. There are lots of alternatives to Leaflet, but most require an API key to use.

## As code
Leaflet consists of JavaScript and CSS code libraries which power the ways your web browser interprets and interacts with geospatial data & displays colors and style. For instance, when you double click a map to zoom in, Leaflet is at work. When you add data to your map, Leaflet assigns it a default color. And because Leaflet is open-source, the code is hugely customizable and extensible. This means you can re-mix the code all you want — which you will do in this workshop. [Here are some examples](https://leafletjs.com/plugins.html) of Leaflet-based plugins to give you some idea of the variety of added functionality that comes from the community of developers.


<!-- ```html
<html>

<head>

  <title>Boilerplate</title>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
    integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin="" />

  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"
    integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>

</head>

<body>

  <div id="mapid" style="height: 100%;"></div>

  <script>
   
   var mymap = L.map('mapid').setView([45.50, -73.58], 13);

   var Stadia_Outdoors = L.tileLayer('https://tiles.stadiamaps.com/tiles/outdoors/{z}/{x}/{y}{r}.{ext}', {
	minZoom: 0,
	maxZoom: 20,
	attribution: '&copy; <a href="https://www.stadiamaps.com/" target="_blank">Stadia Maps</a> &copy; <a href="https://openmaptiles.org/" target="_blank">OpenMapTiles</a> &copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors',
	ext: 'png'
}).addTo(mymap);


  </script>

</body>

</html>

``` -->

## In a browser
Take a look at this basic Leaflet map example. You can zoom in, pan around, etc. It’s meant to be displayed in your internet browser or a mobile application, so it loads and responds to you quickly.

<iframe src="./reference/basic-map.html" style="width:100%; height:520px; border:none;"> </iframe>


#### Leaflet Advantages  ⇡
{: .no_toc}
 - Leaflet is free and open-source. For this reason, Leaflet is widely used. 
 - As an open-source code library, Leaflet is hugely customizable. This means you can re-mix the code all you want. 
 - Leaflet is beginner friendly, though you do need to interact with code in order to build your map.
 - Hugely customizable. Leaflet-based plugins to give you some idea of the variety of added functionality that comes from the community of developers. 
 <!-- - In Leaflet, you can [change the CRS](https://leafletjs.com/reference.html#crs) of your map whereas the projection is set in Google Maps and Mapbox.  -->


#### Leaflet Disadvantages ⇣
{: .no_toc}
 - You'll need to work with code in a code editor. This can introduce a semi-steep learning curve, but you can truly create a basic webmap in a few hours with no prior knowledge. 
 - You'll need a place to store your map and map data. Github can work. Think about how you'll be displaying your end product. Will it be embedded on a website? 
<!--could do a tutorial thats like lets make a map and add data to github and make github page-->