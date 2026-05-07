---
layout: default
title: Data Sources
nav_order: 1
parent: What is Spatial Data?
---
# Data Sources
{: .no_toc}

Now that you understands what spatial data is and the different formats it comes in, you may be wondering *Where, then, do you find spatial data?* Maybe you already have some, maybe you’re still searching. A lot of spatial data is accessible via the internet, albeit under different licenses.

This page outlines some places to look for data. 

<details open markdown="block">
  <summary>
    On this page:
  </summary>
  {: .text-delta }
 - TOC
{:toc}
</details>
----

TAILOR THIS PAGE DIGITAL HUMANITIES SOURCES
{: .warn}

### Historical Data
- [Borealis](https://borealisdata.ca/dataverse/HGIS?q=&types=dataverses%3Adatasets&sort=dateSort&order=desc&page=1)
- MORE?? say more on this



### Libraries, Municipal portals, and Governmental agencies 
Municipal and governmental agencies local to your project are also great places to begin looking. For example, see for Vancouver the [Vancouver Open Data Portal](https://opendata.vancouver.ca/pages/home/), [Data BC](https://catalogue.data.gov.bc.ca/) for Provincial data, and [Natural Resources Canada](https://natural-resources.canada.ca/science-data/data-analysis/geoca) or [here](https://natural-resources.canada.ca/science-data/data-analysis/geospatial-data-tools-services/geospatial-data-tools-services) for national resource data. Many Canadian cities have their own municipal open data source, though downloading the data will be different depending on the platform used by each city (see our workshop on [Tools and Workflows](https://ubc-library-rc.github.io/gis-tools-workflows/content/downloading-data.html) for guidance).  

### Free and open source context layers
[Natural Earth](https://www.naturalearthdata.com/downloads/), which we will use today, provides  free, public domain raster and vector data at a global scale. For example, you can download country and state outlines (and from various state-based perspectives), rivers/lakes/reservoirs, oceans and coastlines, and landmasses. You can also download hillshade data from Natural Earth whose symbology you can adjust in QGIS to show topography. This makes it an excellent resource for simple reference mapping for academic publication.


### World (historical) data
The [Humanitarian Data Exchange](https://data.humdata.org/) contains lots of useful global data. [WorldClim](https://worldclim.org/) publishes historical climate data such as precipitation and temperature, which you can download as raster datasets. For free and open-source infrastructural data, see [Open Street Maps (OSM)](https://www.openstreetmap.org/#map=11/49.2151/-123.0393). Refer to our [Plugins in QGIS Workshop](https://ubc-library-rc.github.io/gis-plugins-qgis/content/extracting-osm-data.html) for a demonstration of how to extract and download OSM data or use it as a basemap for your maps. 

### Satellite Imagery
Satellite imagery can often be downloaded directly from providers. For example, download Sentinel data from the [Copernicus Browser](https://browser.dataspace.copernicus.eu/?zoom=5&lat=50.16282&lng=20.78613&demSource3D=%22MAPZEN%22&cloudCoverage=30&dateMode=SINGLE). If you're using QGIS, the [SRTM-Downloader](https://plugins.qgis.org/plugins/SRTM-Downloader/) plugin is a handy tool to download NASA data for a specific area of interest directly from within your GIS interface. If you are a UBC student, staff, or faculty, you can [request a Planet account](https://researchcommons.library.ubc.ca/planet-imagery/) to gain access to much more imagery. Refer to our [Project Design workshop and resource](https://ubc-library-rc.github.io/gis-spatial-stories/content/resources-for-data-assembly.html) for important considerations as you search, download, store, and use data.


## Creating your own
Finally, you can always create your own vector layers, or create new shapefiles within a GIS by tracing existing data. We will discuss data creation and editing further on another day. 

If you are working with historical or physical maps and want to digitize them or otherwise create spatial data using them as template, see our workshop on [georeferencing](../day3/georeferencing-overview.md) for more. We will discuss georeferencing more later in the week. 


#### Data Finding Guides
- [Concordia's Guide](https://www.concordia.ca/library/guides/geospatial-data/geodata.html)
- ADD MORE