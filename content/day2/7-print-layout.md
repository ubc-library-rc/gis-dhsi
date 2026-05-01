---
layout: default
title: 5. Create a map
nav_order: 5
parent: Reference Mapping
---
# Create a map: Print Layout
{: .no_toc}

Once you are satisfied with your layer symbology, it’s time to create a **Print Layout**. A Print Layout in QGIS is like a drawing board where you add the map you created, as well as other elements like a north arrow, legend, scale bar, text boxes, and other marginalia. You can create multiple Print Layouts per QGIS project. By giving each Print Layout you make a unique name, and saving it (and your QGIS project) regularly, you can return to a Print Layout from the at any time (Project menu –> Layouts) and continue working.


See The QGIS user guide here for a comprehensive introduction to the [QGIS Print Layout](https://docs.qgis.org/3.40/en/docs/training_manual/map_composer/map_composer.html).


<details open markdown="block">
  <summary>
    On this page:
  </summary>
  {: .text-delta }
 - TOC
{:toc}
</details>
----

## Create a new Print Layout

To Do
{: .label .label-green } 
Create a new **Print Layout** by going the Project menu, and down to "New Print Layout". Call it "Montreal".
<img src="./images/print1.png" style="width:100%">
Alternatively, you can click the Print Layout icon in the Toolbar. 
<img src="./images/print2.png" style="width:5%">

This will open the **Print Layout** window. It looks quite similar to the main QGIS interface, so be careful not to edit the wrong thing. Notice, too, that once you've clicked into the Print Layout window, the menu at the top of your screen changes. 

<img src="./images/print3.png" style="width:100%">

## Set Page properties
**Page Properties** govern the orientation and dimensions of the Print Layout, or page. Depending on your publication platform, you might already know your layout constraints. Journals or book publishers will give you max and min dimensions for figures, as well as often dictate what file form they want them in (`.png`, `.jpg`, `.pdf`, or, often, an `.svg` or `.ai` file). For example, when making maps for books, the largest dimensions might be 4 x 6 inches. 

To change the dimensions of the page, go to "Page Properties..." by right-clicking anywhere on the page's whitespace. You can also find Page Properties in the **Layout** menu at the top of your screen. 

<img src="./images/print4.png" style="width:100%">


To Do
{: .label .label-green }
Let's set the page dimensions for today's map to be A4. We'll keep the orientation set to Landscape. 

To change the dimensions, click the **Size** drop-down options and select "A4". To set custom dimensions, choose "Custom" size at the very bottom of the drop-down. This will activate the Height and Width input boxes. If setting a custom size via Height and Width, remember to include the units for these dimensions. In this way, you can set very specific dimensions depending on the criteria of your publisher.

<img src="./images/print5.png" style="width:100%">


Note: If you set smaller dimensions than the default, your Print Layout—the white page juxtaposed to the grey background—will get smaller. To zoom it in so you can see your workspace, drag two fingers diagonally or scroll to enlarge the amount of space your Print Layout takes up on the screen. If you change the size of your Print Layout after you've already added a map, remember to adjust the map size; only what is contained within the Print Layout will be exported. 

<br>

## Add items to the Print Layout

At minimum, apart from the map itself, a Print Layout should have a title, scalebar, north arrow, and map author/data source. A legend is required if you have any layers added to your map that aren't reference layers or that need explanation. 

We can add items using the icons on the left-hand vertical toolbar, but I find these difficult to interpret. For this reason, I default to adding items from the **Add Items menu**. 

<img src="./images/print6.png" style="width:90%">



<!-- 

decide whether to make this full like [Reference Mapping documentation o](https://ubc-library-rc.github.io/gis-reference-mapping/content/hands-on5.html)r abridged like [Thematic mapping documentation. ](https://ubc-library-rc.github.io/gis-thematic-mapping/content/hands-on6.html) -->