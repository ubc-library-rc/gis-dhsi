---
layout: default
title: GIS Overview
nav_order: 1
parent: Day 2
---
# Geographic Information Systems (GIS)

**Learning Objective 1: Understand what a GIS is, and the advantages to using QGIS.**


**GIS** is an abbreviation for **G**eographic **I**nformation **S**ystem. A nice description of GIS that provides a bit of relevancy comes from QGIS's [*A Gentle Introduction to GIS*](https://docs.qgis.org/3.10/en/docs/gentle_gis_introduction/introducing_gis.html):

  >*Just as we use a word processor to write documents and deal with words on a computer, we can use a GIS application to deal with spatial information on a computer*

With that in mind, there are 3 main forms of GISs:

 1. **Utilities and Services (tasks)** - Scripts and programming libraries that manipulate spatial data in specific ways. For example, [**geocoding**](https://desktop.arcgis.com/en/arcmap/latest/manage-data/geocoding/what-is-geocoding.htm) services geolocate a set of points based on address or coordinate attribute data. For example, [MMQGIS](https://plugins.qgis.org/plugins/mmqgis/) is a QGIS plugin which contains a tool for geocoding. 

2. **Desktop (analyses)** - Software that provides a suite of tools for processing and spatially analyzing data. In other words, GIS applications you interact with through a graphical user interface from a computer. Examples include the QGIS desktop app we will use today and Esri ArcGIS Pro. GRASS is another GIS. 

3. **Infrastructure (management)** - Server and web resources that manage, curate, and distribute collections of spatial data. While Esri offers Server web services with ArcGIS Online, many [open source GIS servers](https://mapscaping.com/open-source-gis-servers/) are out there. 



There are a variety of GIS available, some proprietary and some free and open source. Free and open source means... It is for this reason that Research Commons workshops on GIS and Mapping use QGIS, a popular free and open-source GIS you can download directly to your computer. 



<br>

-----

<img src=".../images/QGIS-logo.png" style="width:30%">

[QGIS](https://qgis.org/) is a popular desktop GIS software, and considered a free and open source software (FOSS) with a very active developer community. Take a moment to browse their website.

## QGIS Advantages  ⇡

 - QGIS is free and open source, meaning you can download it directly from the web to your personal computer. 
 - QGIS runs on Windows, Mac, Linux, operating systems, meaning you don't need a specific kind of device to use it. Some proprietary and costly software, such as ArcGIS, only run on Windows computers making it difficult to use without specialized equipment. 
 - QGIS has extensive online documentation, including a comprehensive official [User Guide](https://docs.qgis.org/3.40/en/docs/user_manual/index.html) *and* [Training Manual](https://docs.qgis.org/3.40/en/docs/training_manual/index.html), as well as numerous YouTube and internet resources/tutorials created by users like you. 
 - QGIS has an intuitive interface which can be customized by the user. 
 - QGIS has an active development and user communities, meaning people are constantly posing and answering questions on platforms such as Reddit,  StackExchange, and YouTube. This makes troubleshooting a whole lot easier. There is also an annual [QGIS User Conference](https://uc2026.qgis.org/activities/)!
 - QGIS has a robust [plugin](https://plugins.qgis.org/) repository for extended functionality. This means the application you download to begin with doesn't contain every single tool available, just the necessary and commonly used ones. 

## QGIS Disadvantages ⇣

 - Most recent features can be buggy, which is why we recommend always downloading the latest Long Term Release, often small hyperlink below main download button. 
 - Plugins lack standardized documentation as they are largely user-community developed and contributed
 - Troubleshooting often amounts to searching the web, though this is an important skill to have as a cartographer. 
 - Not ideal for more elaborate spatial analysis or network analysis workflows. 


## QGIS Resources 
{: .no_toc} 
QGIS itself has extensive online documentation, including a robust [User Guide](https://docs.qgis.org/3.40/en/docs/user_manual/index.html) *and* [Training Manual](https://docs.qgis.org/3.40/en/docs/training_manual/index.html). 
    
QGIS also has a vibrant user community, with answers to nearly any question you might have only a web search away. Many helpful tutorial demonstrations can be found on Youtube. For instance, [CWU Geography](https://www.youtube.com/@cwugeography3290) offers especially clear and helpful content, but there are many, many others. 


- [Intro to Map Production with QGIS](https://ubc-library-rc.github.io/gis-intro-qgis/)
- [Reference Mapping with QGIS](https://ubc-library-rc.github.io/gis-reference-mapping/)
- [Thematic Mapping with QGIS]( https://ubc-library-rc.github.io/gis-thematic-mapping/)
- [Tools and Workflows in QGIS](https://ubc-library-rc.github.io/gis-tools-workflows/).
- [Plugins with QGIS](https://ubc-library-rc.github.io/gis-plugins-qgis/)


The best way to learn QGIS is through the experience that comes with hands-on practice. QGIS has with a medium learning curve, especially if you’ve never used a GIS before. However, don’t let this dissuade you! The abundance of QGIS-official and unofficial documentation means you can tailer your learning experience to your interests and the specific needs of your project.