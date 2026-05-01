---
layout: default
title: 1. Gathering Data
nav_order: 1
parent: Reference Mapping
---
# Gathering Data
{: .no_toc}

Yesterday, you learned about spatial data and where to find it. Today, we'll practice visualizing spatial data with a GIS. 

<!-- In the morning, we will practice making a reference map of Montreal's historic public bath houses. In the afternoon, we'll work with pre-prepared historic data from the public history project *[Montréal, l’avenir du passé (MAP)]([Montréal, l’avenir du passé (MAP)](https://mun.ca/mapm/fra/accueil_cadre.html))* (*Montréal, The Future of the Past*) to create thematic maps visualizing demographic data from the 1880s. Tomorrow we'll return to the data used this morning as we explore common tools and workflows in QGIS.  -->


This morning, we'll acquaint ourselves with the QGIS interface by making a reference map of historic public bath houses in Montreal. However, to give this dataset – put together by Alex Alisauskas — some context, we'll need some spatial data representing geographic features: the city of Montreal, Canadian provinces, green spaces, and water features. We could add a lot more to this list, but for today let's keep it simple. 

If you look in the `dhsi-workshop/Day2` folder you'll see subfolders for both this morning and this afternoon. Inside  `dhsi-workshop/Day2/reference-mapping` you'll see one shapefile file for the city of Montreal but nothing else. Because in the real world data is seldom provided neatly packaged, we'll begin by guiding you in downloading and synthesizing vector data geographic data from multiple online sources.

----



## Montreal Historic Bath Houses

- [Montreal Public Baths](https://docs.google.com/spreadsheets/d/11GN2Al7_QNFpcOxBhjVXv0KuP-yv44F1zQZ1KxIE7EM/edit?gid=0#gid=0)
Although there is a lot of spatial data available for download that with some modification (using tools and workflows largely introduced tomorrow) can suit a variety of mapping purposes, you will doubtless run into situations where you have to create your own data. For example, maybe you want to plot significant sites visited by the protagonist of a novel, or the opera houses frequented by a notable musician. Recalling yesterday's discussion of vector data formatting - Alex will now introduce the dataset and explain her process and considerations for making it. Then, guide us in exporting it as a `.csv` called `public-baths`. 

<img src="./images/gathering0.png" style="width:100%">

 
## Basemap Data
Remember, move each dataset you download to `dhsi-worshop/Day2/reference-mapping` and *unzip it* there if a compressed folder. You will notice very quickly the varying degrees of data management - naming. keep this in mind when you create your own data or work on your own project. If you have any trouble downloading the data, we've created a `backup-data` folder with all the necessary files zipped. just unzip before you use. 
<!-- Additionally, of a `.geojson` file feel free to directly rename it. (You can rename shapefiles too, but there will be a number of sidecar files you'll also have to rename to match.) -->
   
Download the following shapefiles: 

- [Provincial boundaries](https://www12.statcan.gc.ca/census-recensement/2021/geo/sip-pis/boundary-limites/index2021-eng.cfm?year=21)


- For water features, we want both the [Hydrography for the wider Montreal Metro Area](https://donnees.montreal.ca/dataset/hydrographie-communaute-metropolitaine-montreal) *as well as* [Hydrography for Montreal agglomerations](https://donnees.montreal.ca/dataset/hydrographie). 


- [Parks and Green Spaces](https://donnees.montreal.ca/dataset/grands-parcs-parcs-d-arrondissements-et-espaces-publics)



### Download Provincial Boundaries
We'll download [provincial boundaries](https://www12.statcan.gc.ca/census-recensement/2021/geo/sip-pis/boundary-limites/index2021-eng.cfm?year=21) from census data hosted by the Government of Canada's data portal. 

2021 Census – Boundary files

<img src="./images/gathering1.png" style="width:100%">

<img src="./images/gathering2.png" style="width:100%">


<br>

### Download Water Features
We'll download two sets of water features from the City of Montreal's data portal, one for the [City of Montreal](https://donnees.montreal.ca/dataset/hydrographie) and one for the [Montreal Metro area](https://donnees.montreal.ca/dataset/hydrographie-communaute-metropolitaine-montreal). Use the same process for each. MAKE SURE YOU DOWNLOAD `.SHP`. They are listed in different orders for each



<img src="./images/gathering3.png" style="width:100%">

<br>
<img src="./images/gathering4.png" style="width:100%">


<!-- The same process [Hydrography for the wider Montreal Metro Area](https://donnees.montreal.ca/dataset/hydrographie-communaute-metropolitaine-montreal) *as well as* [Hydrography for Montreal agglomerations](https://donnees.montreal.ca/dataset/hydrographie).  -->



### Download Water Features
We'll download [Parks and Green Spaces](https://donnees.montreal.ca/dataset/grands-parcs-parcs-d-arrondissements-et-espaces-publics) also from the city of Montreal's data portal. Note that the format for shapefile will show ZIP. 

<img src="./images/gathering5.png" style="width:100%"> 
<img src="./images/gathering6.png" style="width:100%"> 



BE SURE TO MOVE ALL COMPRESSED FOLDERS TO XYZ FOLDER< AND > UNZIP EVERYTHING. stop and make sure everyone has. - have them confer with small groups. 



note: What's given is an edited version of administrative boundary file located both on the [montreal portal](https://donnees.montreal.ca/dataset/limites-administratives-agglomeration)  as well as govt of canada. 