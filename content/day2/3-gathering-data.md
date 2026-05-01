---
layout: default
title: 1. Gathering Data
nav_order: 1
parent: Reference Mapping
---
# Gathering Data
{: .no_toc}

Yesterday, you learned about spatial data and where to find it. Today, we'll practice visualizing spatial data with a GIS. In the morning morning we will practice making a reference map of Montreal's historic bath houses. Because in the real world data is seldom provided neatly packaged, you will be guided in downloading and synthesizing vector data geographic data from multiple online sources. In the afternoon, we'll work with pre-prepared historic data from the public history project *[Montréal, l’avenir du passé (MAP)]([Montréal, l’avenir du passé (MAP)](https://mun.ca/mapm/fra/accueil_cadre.html))* (*Montréal, The Future of the Past*) to create thematic maps visualizing demographic data from the 1880s. Tomorrow we'll return to the data used this morning as we explore common tools and workflows in QGIS. 


---
## Data for Reference Mapping
This morning, we'll acquaint ourselves with the QGIS interface by adding and modifying layers, and making a reference map. We will be mapping historic bath houses across the city of Montreal — a dataset put together by Alex Alisauskas. We'll also want some geographic context: provinces, the city of Montreal, water features, and green spaces. 

If you look in the `dhsi-workshop/Day2` folder you'll see subfolders for both this morning and this afternoon. Inside  `dhsi-workshop/Day2/reference-mapping` you'll see one `.geojson` file for the city of Montreal and a QGIS project. ??? Or - no project - ask them to launch qgis. The rest of the data we'll download together. (should i have a backup folder incase. ) 



### Downloading data

To Do
{: .label .label-green }    

- [Montreal Public Baths](https://docs.google.com/spreadsheets/d/11GN2Al7_QNFpcOxBhjVXv0KuP-yv44F1zQZ1KxIE7EM/edit?gid=0#gid=0)
Although there is a lot of spatial data available for download that with some modification (using tools and workflows largely introduced tomorrow) can suit a variety of mapping purposes, you will doubtless run into situations where you have to create your own data. For example, maybe you want to plot significant sites visited by the protagonist of a novel, or the opera houses frequented by a notable musician. Recalling yesterday's discussion of vector data formatting - Alex will now introduce the dataset and explain her process and considerations for making it. Then, guide us in exporting as `.csv`. 

Maybe also demo creating point in geojson.io??? 

 
### Spatial data
Remember, move each dataset you download to `dhsi-worshop/Day2/reference-mapping` and *unzip it* there if a compressed folder. Additionally, of a `.geojson` file feel free to directly rename it. (You can rename shapefiles too, but there will be a number of sidecar files you'll also have to rename to match.)

To Do
{: .label .label-green }    

- [provincial boundaries](https://www12.statcan.gc.ca/census-recensement/2021/geo/sip-pis/boundary-limites/index2021-eng.cfm?year=21)
(tomorrow: tools and workflows: select quebec and export out)

- For water features, we want both [hydrography for the wider Montreal Metro Area](https://donnees.montreal.ca/dataset/hydrographie-communaute-metropolitaine-montreal) *as well as* [Hydrography for Montreal agglomorations](https://donnees.montreal.ca/dataset/hydrographie). 
<!-- CARTO_DRA_EAU_JOUR that layer plus the one for the metro community. -->

- ?perhaps public access rivers `rivespubliquesaccessibles` [Rivers](https://donnees.montreal.ca/dataset/rive-publique/resource/473df7a0-7fd3-4f33-afae-03b21c1d7f40)[water courses](https://donnees.montreal.ca/fr/dataset/cours-d-eau-et-fosse) 

- [Parks and Green Spaces](https://donnees.montreal.ca/dataset/grands-parcs-parcs-d-arrondissements-et-espaces-publics)



**3. Create a point over Montreal** or UdeM
Finally, we will create a point over Montreal. To do this, will use <a href="https://geojson.io/#map=2/0/20" target="_blank">geojson.io</a>, an online platform where you can click to create simple point, line, and polygon features which can then be downloaded and uploaded to a GIS. 

1. Go to <a href="https://geojson.io/#map=2/0/20" target="_blank">geojson.io</a> 

2. Simply type "Montreal" in the search bar and the webmap should zoom to the desired location. 
<img src="./images/geojson-io_20251113.png" style="width:100%">

3. Click the drop-pin icon. Your cursor should turn into a cross hair. Now click on the map, exactly where the drop-pin for Montreal is already given.     
<img src="./images/geojson-drawpoint_20251113.png" style="width:100%"> 

4. Once you click, you will notice some geoJSON code appears on the right-hand panel. This is the geoJSON that stores a single point. Click **Save** in the upper left-hand corner, and save your new point layer as either a `geojson` (notice, however, you can save as a shapefile or another file format as well). Once the file is downloaded, ***move it to your `dhsi-worshop/Day2/reference-mapping` folder. You may need to rename it to `montreal` rather than `map.geojson` which is the default. 
<img src="./images/geojson-save_20251113.png" style="width:100%">

 

