---
layout: default
title: What is GIS?
nav_order: 2
parent: Day 2
---
# Geographic Information Systems (GIS)

**GIS** is an abbreviation for **G**eographic **I**nformation **S**ystem. A nice description of GIS that provides a bit of relevancy comes from QGIS's <a href="https://docs.qgis.org/3.44/en/docs/gentle_gis_introduction/introducing_gis.html" target="_blank">*A Gentle Introduction to GIS*</a>:

  >*Just as we use a word processor to write documents and deal with words on a computer, we can use a GIS application to deal with spatial information on a computer*


A Geographic Information System (GIS) works with data that is tied to a location on Earth. As we learned yesterday, this type of data is often referred to as "spatial data", "geospatial data", or even "GIS data", and is spatially referenced using location information — most commonly *geographic coordinates*. A GIS uses this location information to project a geospatial file into a virtual geographic space where it can then be visualized and manipulated.

<!-- With that in mind, there are 3 main forms of GIS, most often working together:

1. **Utilities and Services (tasks)** - Scripts and programming libraries that manipulate spatial data in specific ways. For example, [**geocoding**](https://desktop.arcgis.com/en/arcmap/latest/manage-data/geocoding/what-is-geocoding.htm) services geolocate a set of points based on address or coordinate attribute data. For example, [MMQGIS](https://plugins.qgis.org/plugins/mmqgis/) is a QGIS plugin which contains a tool for geocoding. 

2. **Desktop (analyses)** - Software that provides a suite of tools for processing and spatially analyzing data. In other words, GIS applications you interact with through a graphical user interface from a computer. Examples include the QGIS desktop app we will use today and Esri ArcGIS Pro. GRASS is another GIS. 

3. **Infrastructure (management)** - Server and web resources that manage, curate, and distribute collections of spatial data. While Esri offers Server web services with ArcGIS Online, many [open source GIS servers](https://mapscaping.com/open-source-gis-servers/) are out there.  -->


There are a variety of GIS available, some proprietary like Esri ArcGIS, and others free and open source like [OpenJUMP](http://www.openjump.org/){:target="_blank"}, [GRASS](https://grass.osgeo.org/){:target="_blank"}, and [QGIS](https://qgis.org/){:target="_blank"}. [Free and open source software (FOSS)](https://en.wikipedia.org/wiki/Free_and_open-source_software){:target="_blank"} means you can download and use it for free, as well as view and modify the software's source code. For this reason, this DHSI workshop will center free and open source software wherever possible. Any propriety tools and platforms introduced will be free to use. 



<br>

-----

<img src="./images/QGIS-logo.png" style="width:30%">

[QGIS](https://qgis.org/){:target="_blank"} is a popular desktop GIS software, and considered a [free and open source software (FOSS)](https://en.wikipedia.org/wiki/Free_and_open-source_software){:target="_blank"} with a very active developer community. 

## QGIS Advantages  ⇡
- QGIS is free and open source, meaning you can download it directly from the web to your personal computer and view its source code. 
- QGIS runs on Windows, Mac, and Linux operating systems, meaning you don't need a specific kind of device to use it. (Some proprietary and costly software, such as ArcGIS, only runs on Windows.) 
- QGIS has extensive online documentation, including a comprehensive official [User Guide](https://docs.qgis.org/3.44/en/docs/user_manual/index.html){:target="_blank"} *and* [Training Manual](https://docs.qgis.org/3.44/en/docs/training_manual/index.html){:target="_blank"}. 
- QGIS has an active development and user communities, meaning people are constantly posing and answering questions on platforms such as Reddit,  StackExchange, and YouTube. This makes troubleshooting a whole lot easier. There is also an annual [QGIS User Conference](https://uc2026.qgis.org/activities/){:target="_blank"}!
- QGIS has an intuitive and customizable interface. While navigating any new application can be overwhelming, QGIS has a lot less going on visually than ArcGIS Pro making it quite a good starting place for  newcomers to GIS. 
- QGIS has a robust [plugin](https://plugins.qgis.org/){:target="_blank"}{:target="_blank"} repository for extended functionality. This means the application you download to begin with doesn't contain every single tool available, just the necessary and commonly used ones. 


## QGIS Disadvantages ⇣
- Most recent features can be buggy, which is why we recommend always downloading the latest Long Term Release.
- Plugins lack standardized documentation as they are largely user-community developed and contributed.
- Troubleshooting often amounts to searching the web, though this is an important skill to have as a cartographer. 
- Performing more elaborate analysis workflows in QGIS requires more expertise, while in ArcGIS, tools and documentation for such work can be more user-friendly.

#### QGIS Resources 
{: .no_toc} 
QGIS itself has extensive online documentation, including a robust [User Guide](https://docs.qgis.org/3.44/en/docs/user_manual/index.html){:target="_blank"} *and* [Training Manual](https://docs.qgis.org/3.44/en/docs/training_manual/index.html){:target="_blank"}. 
    
QGIS also has a vibrant user community, with answers to nearly any question you might have only a web search away. Many helpful tutorial demonstrations can be found on Youtube. For instance, [CWU Geography](https://www.youtube.com/@cwugeography3290) offers especially clear and helpful content, but there are many, many others. 

The best way to learn QGIS is through the experience that comes with hands-on practice. QGIS has with a medium learning curve, especially if you’ve never used a GIS before. However, don’t let this dissuade you! The abundance of QGIS-official and unofficial documentation means you can tailer your learning experience to your interests and the specific needs of your project.






<!-- Whereas yesterday you learned about spatial data and where to find it, today you'll practice gathering, loading, and symbolizing spatial data. -->