---
layout: default
title: Day 4
nav_order: 5
has_children: true
---
# Day 4: Web Mapping 

Today we will explore web maps (aka webmaps) and web mapping (aka webmapping). Web maps are a means of dynamically and interactively visualizing geospatial data. Web maps can be hosted on the web and shared with others via a link. Today, you will learn how to create web maps in 3 different manners: 

1. **online**, through platforms such as [uMap](https://umap.openstreetmap.fr/en/){:target="_blank"} and [Google MyMaps](https://www.google.com/maps/about/mymaps/){:target="_blank"};
2. in **QGIS**, using the [qgis2web plugin](https://plugins.qgis.org/plugins/qgis2web/){:target="_blank"}; and
3. with **code**, powered by [Leaflet](https://leafletjs.com/){:target="_blank"}.

Each of these methods of web mapping has its advantages and disadvantages which we will discuss. Moreover, while we emphasize that web mapping can be done entirely online without any coding necessary, it's useful to have a general understanding of how a web map works. To this end, we will break down the "anatomy" of a web map in a code editor in order to observe how the various components of a web map work together. By the end of the day, you will be equipped with the fundamental knowledge and skills to begin web mapping on your own. 


<br>

#### **Morning Session** 9am - 12pm
- Web mapping **online** with [uMap](https://umap.openstreetmap.fr/en/){:target="_blank"} and [Google MyMaps](https://www.google.com/maps/about/mymaps/){:target="_blank"}
- Webmapping with QGIS using the [qgis2web plugin](https://plugins.qgis.org/plugins/qgis2web/#plugin-about){:target="_blank"}


<!-- Hands on activity 1 - small groups assigned different datasets to map using either GoogleMy Maps or uMap 
{: .warn} -->

<br>

#### **Afternoon Session** 1:30pm - 4pm
- The Anatomy of a Webmap
- Hands on with [Leaflet](https://leafletjs.com/){:target="_blank"}
- Hosting your webmap online with [GitHub](https://github.com/) {:target="_blank"}

<!-- 
activity could be - run selection of data in qgis -> export as geojson - then wrap as javascript and add to project. multipart vs. part be aware for points. solve using centroid.
{: .warn} -->

<br>



## What we will make

Below are examples of webmap made with uMap, Google MyMaps, and Leaflet. 


<iframe style="width: 100%; height: 520px; border: 0;" allowfullscreen src="//umap.openstreetmap.fr/en/map/toronto-public-art_1377239?scaleControl=false&miniMap=false&scrollWheelZoom=false&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#11/43.72/-79.42"></iframe>
<!-- 
<p style="font-size:11pt;"><a href="//umap.openstreetmap.fr/en/map/toronto-public-art_1377239?scaleControl=false&miniMap=false&scrollWheelZoom=true&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#11/43.72/-79.42" target="_blank">View in full screen</a></p> -->
<sub>[See full screen](//umap.openstreetmap.fr/en/map/toronto-public-art_1377239?scaleControl=false&miniMap=false&scrollWheelZoom=true&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#11/43.72/-79.42){:target="_blank"}</sub>  



<br>

<iframe src="https://www.google.com/maps/d/embed?mid=11gHGxEF2Uxx7zbn00htegHybzWBS3ro&ehbc=2E312F&noprof=1" style="width:100%; height:520px; border:none;"></iframe>
<sub>[View in Full Screen](https://www.google.com/maps/d/embed?mid=11gHGxEF2Uxx7zbn00htegHybzWBS3ro&ehbc=2E312F&noprof=1){:target="_blank"}</sub> 

<br>

<iframe src="./reference/leaflet-example.html" style="width:100%; height:520px; border:none;"> </iframe>
<sub>[View in Full Screen](./reference/leaflet-example.html){:target="_blank"}</sub> 


<br>

<!-- 
<iframe src="https://lilydemet.github.io/qgis2web-example-map/" style="width:100%; height:520px; border:none;"> </iframe>
<sub>[View GitHub repo](https://github.com/lilydemet/qgis2web-example-map)</sub>    -->





## Data
We will be working from the `dhsi-workshop/Day4` folder. Inside, you will see today's data further organized into 3 subfolders relevant to webmapping online, webmapping with Leaflet, and webmapping with QGIS respectively.

We will webmap using data on [Public Art](https://open.toronto.ca/dataset/public-art/){:target="_blank"} and [Heritage Conservation Districts](https://open.toronto.ca/dataset/heritage-conservation-districts/){:target="_blank"} from the [City of Toronto's open data portal](https://open.toronto.ca/catalogue/){:target="_blank"}. This data is licensed under the [Open Government Licence - Toronto](https://open.toronto.ca/open-data-licence/){:target="_blank"}, meaning we can modify and adapt the data! The datasets have been reformatted to be legible to the various tools and platforms we will work with today. The QGIS project and data you'll recognize from our reference mapping in Day 2. We've also included an additional dataset of [community gardens](https://donnees.montreal.ca/fr/dataset/jardins-communautaires){:target="_blank"} from the City of Montreal open data portal.  


<!-- activity ADD GREEN SPACES OR SOMETHING ELSE TO FOLDER AS GEOJSON SO THEY CAN WRAP AS VARIABLE ETC... or have them download from web
{: .warn} -->

<!-- - [Green Spaces](https://open.toronto.ca/dataset/green-spaces/)
- [City Wards](https://open.toronto.ca/dataset/city-wards/)
- [Regional Municipal Boundary](https://open.toronto.ca/dataset/regional-municipal-boundary/) -->

<!-- 
The QGIS Project includes province (and water features?), data from government of canada as well as - ?? from natural earth data. Data from The Government of Canada is licensced under the Open Government Licence - Canada; Data from [Natural Earth](https://www.naturalearthdata.com/) is [public domain](https://www.naturalearthdata.com/about/terms-of-use/) and therefore free to use.   -->



<br><br>



### Webmapping in DH research
- [Designing for discovery: using web maps in the digital humanities](https://dhq.digitalhumanities.org/vol/19/4/000819/000819.html){:target="_blank"}
- [The Polyrhythm Project](https://polyrhythm.humdrum.org/overview/){:target="_blank"} created [maps](https://polyrhythm.humdrum.org/maps/){:target="_blank"} for their [Corpus](https://maps.polyrhythm.humdrum.org/corpus/){:target="_blank"}, [Composers](https://maps.polyrhythm.humdrum.org/composers/#4/49.43/10.40){:target="_blank"}, and [Timeline](https://maps.polyrhythm.humdrum.org/timeline/){:target="_blank"}.
- [Don Valley Historical Map Project](https://utoronto.maps.arcgis.com/apps/webappviewer/index.html?id=6055c7fbccdf44ac911a4e13b34a825c){:target="_blank"}
- [Mapping Prejudice](https://mappingprejudice.umn.edu/){:target="_blank"}