---
layout: default
title: Webmapping Online
nav_order: 2
parent: Day 4
has_children: true
---
# Online Platforms for Web Mapping
Online platforms offer browser-based tools for making web maps. This option requires *no coding* and poses the lowest learning barrier.  We will now introduce 2 online platforms for webmapping: [Google MyMaps](https://www.google.com/maps/about/mymaps/) and [uMap](https://umap.openstreetmap.fr/en/). After demonstrating how to add and style layers in each interface, you will then have a chance to choose one to make a map with. 

<!-- To Do
{: .label .label-green } -->
Before we begin, please ensure you have an account with both Google and uMap. These are both free accounts. 

----


## Google MyMaps
We recommend Google as a web mapping platform for its *Google MyMaps service  only*. With [Google MyMaps](https://www.google.com/maps/about/mymaps/), you can create simple maps with drop pin locations or import data layers. Here's an example: 

<iframe src="https://www.google.com/maps/d/embed?mid=11gHGxEF2Uxx7zbn00htegHybzWBS3ro&hl=en&ehbc=2E312F" style="width:100%; height:520px; border:none;"></iframe>

<br>

#### Google Advantages and Disadvantages
{: .no_toc}
 - Google MyMaps is very straightforward to use. If you want to quickly make a map or walking tour, this option might be fore you. 
 - You can adjust the visibility options to enable collaborative editing. Because the Google Maps interface is so widely used, there is an added advantage of MyMaps already being an intuitive platform to potential collaborators and users. 
 - Google MyMaps, as a proprietary service, offers limited customization. 
 - Data privacy is a concern, though you can adjust what attributes are visible on pop-up. However, you might want to check that you've eliminated all identifying or otherwise confidential information from your dataset(s) before uploading them to Google. 
 - Data must be formatted to `.csv` or `.kml`. use [geojson.io](https://geojson.io/#map=2/0/20) to easily convert vector data online from shapefile and geojson format to csv and kml.  
 - While the Google Maps platform offers a panoply of mapping tools including [dynamic maps](https://mapsplatform.google.com/maps-products/dynamic-maps/), you must *be very careful about surreptitious charges*. For example, while the [embed maps API](https://developers.google.com/maps/documentation/embed/get-started?hl=en) is free with unlimited usage, you must sign up for Google Cloud to use it. Google Cloud is only free for 90 days, after which you will be charged $200 monthly. In our opinion, beyond the simple drag-and-drop visualizations offered by Google MyMaps, it is recommended to invest your time and energy in learning a free and open-source option like uMap or Leaflet (detailed below). 


<br>


## uMap
[uMap](https://umap.openstreetmap.fr/en/) is a free and open-source platform that allows you to create web maps using OpenStreetMap (OSM) as your base data. With uMap, you can choose from a variety of basemaps on top of which you can add and customize your own data layers. You can also work collaboratively on a uMap. You can embed your final map into existing websites, or simply share the link to your final map with collaborators and audiences. You can even download your entire map as code! 



<iframe style="width: 100%; height: 520px; border: 0;" allowfullscreen src="//umap.openstreetmap.fr/en/map/toronto-public-art_1377239?scaleControl=false&miniMap=false&scrollWheelZoom=false&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#11/43.72/-79.42"></iframe><p><a href="//umap.openstreetmap.fr/en/map/toronto-public-art_1377239?scaleControl=false&miniMap=false&scrollWheelZoom=true&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#11/43.72/-79.42" target="_blank">See full screen</a></p>


<Br>

#### uMap Advantages and Disadvantages
{: .no_toc}
- uMap is very easy to use. It is an entirely web-based interface and requires no coding or prior expertise in webmapping. 
- You can export your entire project as code and play around with it locally.
- You can embed images in pop-ups. 
- There are extensive customization options for styling layers and markers. 
