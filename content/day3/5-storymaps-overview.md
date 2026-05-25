---
layout: default
title: Story Maps
nav_order: 4
parent: Day 3
has_children: true
---
# Story Maps: making multimedia narratives
{: .no_toc}

Story Maps bring the visiter on a dynamic spatial journey, using multimedia to tell a story that moves (often linearly) through specified locations. Examples of stories that could be told with a narrative map include timelines, travels, and voyages.

#### DH Example Projects using Story Maps
Examples of stories that could be told with a narrative map include timelines, travels, and voyages.

relevance to DH?
{: .warn}

- [Mapping Lost Rivers](https://newsinteractives.cbc.ca/features/2024/daylighting-rivers/)
- See [main page](https://www.lostrivers.ca/)
- [Queer Sapphic New York](https://zhangyuchun17.github.io/Hidden-Constellations/) (Click *on* the arrow).
- knightlab examples 


Story Maps take the form of a website, often combining images, text, video, and static or interactive maps. While you could add multimedia to a website of your own, this afternoon we'll introduce you to 2 platforms that will host a Story Map for you. 



<details open markdown="block">
  <summary>
    On this page:
  </summary>
  {: .text-delta }
 - TOC
{:toc}
</details>


----

## ArcGIS Storymaps
[ArcGIS StoryMap](https://doc.arcgis.com/en/arcgis-storymaps/get-started/what-is-arcgis-storymaps.htm) is a web-based story authoring application that allows you to share your maps in the form of a multimedia narrative. StoryMaps are essentially single-page websites with embedded content. As you will see throughout this workshop, StoryMaps are pretty straightforward to make and can be a great presentation tool.

### Understanding the ArcGIS Online platform  
{: .no_toc}
As an online platform, ArcGIS StoryMap is part of Esri's larger ArcGIS Online suite of proprietary tools. ArcGIS Online is a cloud-based software that allows you to create and organize geospatial projects, which can come in the form of spatial narratives, data files created with desktop GIS applications, interactive web maps, dashboards, and more. Our focus will be on the StoryMaps application, as well as the online mapping tool which we will use to make an interactive map we will then embed in our StoryMap. Understanding the workflow required to upload spatial data into ArcGIS online and create a basic visualization via the online mapping tools is an advantageous skill to have. Furthermore, any map you wish to include in your StoryMap, be it static or dynamic, must be prepared yourself. The only maps you can make from within StoryMaps are "map tours" where locations are selected to correspond to text and/or multimedia documentation. 


### Why Choose ArcGIS Online?
{: .no_toc}
 - No software install necessary
 - Don't have to know how to code
 - No server needed to host your published maps and data
 - Collaborate asynchronously on maps and share them via the web 
 - Easily embed web maps, StoryMaps, and other ArcGIS Online apps in external websites



> #### AGOL Storymaps Advantages  ⇡
> {: .no_toc}
> - Straightforward to learn, with easy drag-and-drop components
> - Produces aesthetic out-of-the box visuals
> - Can contain multimedia, including images, audio, and static maps as well as dynamic maps made with ArcGIS Online
> - See Esri's [Introduction to ArcGIS Storymaps](https://doc.arcgis.com/en/arcgis-storymaps/get-started/what-is-arcgis-storymaps.htm) to get started.
> - The Research Commons also offers a workshop on [StoryMaps and ArcGIS Online](https://ubc-library-rc.github.io/gis-storymaps/). 


> #### AGOL Storymaps Disadvantages ⇣
> {: .no_toc}
> - ArcGIS Online is proprietary, meaning it is not free to use
> - Licensing is a hassle, and collaboration can only occur between people who both own an active license
> - Once your license lapses, your project will disappear
> - You have to make all the maps and graphics yourself, the Storymap is simply the aesthetic container that gathers all the components together


#### Examples
{: .no_toc}
- [Mapping Amazon 2.0](https://storymaps.arcgis.com/stories/144d21045a794cf8b7834b0c49fdd0c0)
- [City of Abbotsford](https://storymaps.arcgis.com/stories/9d2a3452e2a141399ae6226a627b4a36)
- [Isolation Psychogeography](https://storymaps.arcgis.com/stories/4ab243f6d7b3490bbfa884d18a788236)
- [Resilient Woodlands](https://storymaps.arcgis.com/stories/2e02a0b503fb469d8e66fd53a482dffd)


### Supported Data Type of ArcGIS Online
{: .no_toc}
The most common data type that we use is Shapefile. If you have ArcGIS online *organizational account*, you can zip the shapefiles in a folder and upload the zip file to your ArcGIS online account **Content**. Otherwise, if you only have access to *free public account*, convert your shapefiles to other geospatial file formats such as KML or geoJSON before uploading them. You can convert them inside a GIS, or using an online file converter. 

If you have privileges to create content, you can add many types of content as item to ArcGIS online. Please check the [ArcGIS online supported data file here](https://doc.arcgis.com/en/arcgis-online/reference/supported-items.htm).



<br><br>

## Knightlab StoryMap

[Knightlab StoryMap JS](https://storymap.knightlab.com/) is a free and open-source alternative to ArcGIS Storymaps. It is incredibly easy to use and can handle a variety of multimedia. You can also create a timeline with Knightlab [Timeline](https://timeline.knightlab.com/).





discuss specific to digital humanities 
{: .warn}


#### Examples 
{: .no_toc} 
- [Hieronymous Bosch: The Garden of Earthly Delights](https://storymap.knightlab.com/examples/bosch-garden/)
- [Find the drift](https://uploads.knightlab.com/storymapjs/b238a6d62c46c28699e948c1e9d7abc7/findthedrift/index.html) 
<!-- - [Monitering Canada's deforestation](https://ca.nfis.org/ndms/ndms_overview_eng.html)  -->
- [Ancient Rome in Chicago](https://s3.amazonaws.com/uploads.knightlab.com/storymapjs/783a09de8300e1b5f74b99b99acb08ef/ancient-rome-in-chicago/index.html) 
- [Queer Sapphic New York](https://zhangyuchun17.github.io/Hidden-Constellations/) (*Click* on the arrow)

#### Resources for working with Knightlab StoryMap
{: .no_toc}
- [Video introduction to knightlab StoryMap](https://www.youtube.com/watch?v=X33ud7RYZFg) by Cara Marta Messina
- [Workshop on knightlab](https://libguides.hope.edu/storymap) by Victoria Longfield from Hope College
- Another [Workshop](https://dh.sites.gettysburg.edu/toolkit/tools/storymap-js/) on knightlab StoryMap by Gettysburg College
- A [video workshop](https://www.youtube.com/watch?v=ywKH_Ja7sm0) on knightlab's Storymaps by Dr. Anne Ladyem McDivitt of the Alabama Digital Humanities Center
- [Tutorial](https://programminghistorian.org/en/lessons/displaying-georeferenced-map-knightlab-storymap-js) on displaying a georeferenced map on knightlab 
- [Tutorial for making storymap with Knightlab Storymap JS - Barnard](https://github.com/dhc-barnard/tutorials/blob/master/StoryMapJS.md)
- [Tutorial for making timeline with Knightlab Timeline JS - Barnard](https://github.com/dhc-barnard/tutorials/blob/master/TimelineJS.md)
- [Displaying a Georeferenced Map in KnightLab’s StoryMap JS](https://programminghistorian.org/en/lessons/displaying-georeferenced-map-knightlab-storymap-js)


again - not sure what to put in resources dump page or on each relevent intro page?
{: .warn}

----
### TimeMapper
{: .no_toc}

[TimeMapper](https://timemapper.okfnlabs.org/) is another free and open source platform for creating timeline spreadsheet data. TimeMapper is useful if the map is more auxiliary to the timeline. See this [example](https://timemapper.okfnlabs.org/adamrabinowitz/archaeowinetimeliner). Purdue University has a [tutorial](https://library.pfw.edu/timemapper) if this is a tool you're interested in learning. 

### Timeline - different than time mapper? 

also - [timeline](http://timeline.knightlab.com/) 
eg [timeline example](https://timeline.knightlab.com/examples/user-interface/index.html)





http://lab.digital-democracy.org/maplibre-storymap/demo/

https://github.com/digidem/maplibre-storymap



<Br>

#### Resources for StoryMapping
- [The tale of two ArcGIS Online map viewers: functionality guidance](https://www.esri.com/arcgis-blog/products/arcgis-online/mapping/tale-of-two-arcgis-online-map-viewers-functionality-guidance/)
- [ArcGIS Online Relationship Style](https://enterprise.arcgis.com/en/portal/latest/use/style-numbers.htm#ESRI_SECTION1_C7FAB061D60344CAB6AC9A190DAED1D2)
- [Telling the Truth - Data classification](http://uxblog.idvsolutions.com/2011/10/telling-truth.html)
- [Better Breaks Define Your Map’s Purpose](https://www.esri.com/arcgis-blog/products/arcgis-online/mapping/better-breaks-define-your-maps-purpose/)
- [ArcGIS Arcade for Creating Expressions and Coding within your Map](https://storymaps.arcgis.com/stories/e5c8528325c84d56b24afddaa796bfac)