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
Create a new **Print Layout** by going the Project menu, and down to "New Print Layout". Call it "Public Baths".
<img src="./images/layout1.png" style="width:100%">
Alternatively, you can click the Print Layout icon in the Toolbar. 
<img src="./images/layout2.png" style="width:5%">

This will open the **Print Layout** window. It looks quite similar to the main QGIS interface, so be careful not to edit the wrong thing. Notice, too, that once you've clicked into the Print Layout window, the menu at the top of your screen changes. 

<img src="./images/layout3.png" style="width:100%">

## Set Page properties
**Page Properties** govern the orientation and dimensions of the Print Layout, or page. Depending on your publication platform, you might already know your layout constraints. Journals or book publishers will give you max and min dimensions for figures, as well as often dictate what file form they want them in (`.png`, `.pdf`, or, often, an `.svg` or `.ai` file). For example, when making maps for books, the largest dimensions might be 4 x 6 inches. Note that JPEGs are discouraged in favor of PNGs as PNGs store information at a higher resolution. 

To change the dimensions of the page, go to "Page Properties..." by right-clicking anywhere on the page's whitespace. You can also find Page Properties in the **Layout** menu at the top of your screen. 

<img src="./images/layout4.png" style="width:100%">


To Do
{: .label .label-green }
Let's set the page dimensions for today's map to be **A4**. And, let's change the orientation to **Portrait** to better accommodate the extend of our data. To change the dimensions, click the **Size** drop-down options and select "A4". 

<img src="./images/layout5.png" style="width:100%">

*To set custom dimensions, choose "Custom" size at the very bottom of the drop-down. This will activate the Height and Width input boxes. If setting a custom size via Height and Width, remember to include the units for these dimensions. In this way, you can set very specific dimensions depending on the criteria of your publisher.*

*Note: If you set smaller dimensions than the default, your Print Layout—the white page juxtaposed to the grey background—will get smaller. To zoom it in so you can see your workspace, drag two fingers diagonally or scroll to enlarge the amount of space your Print Layout takes up on the screen. If you change the size of your Print Layout after you've already added a map, remember to adjust the map size; only what is contained within the Print Layout will be exported.* 

<br>

## Add items to the Print Layout

At minimum, apart from the map itself, a Print Layout should have a title, scalebar, north arrow, and map author/data source. A legend is required if you have any layers added to your map that aren't reference layers or that need explanation. 

We can add items using the icons on the left-hand vertical toolbar, but I find these difficult to interpret. For this reason, I default to adding items from the **Add Items menu**. 


<img src="./images/layout6.png" style="width:65%">


*Note: If you don't see the Print Layout menu at the top of your screen, make sure you've clicked into Print Layout. If you click back into your main QGIS project, the menu at the top of your screen will change correspondingly.*
<!-- 

decide whether to make this full like [Reference Mapping documentation o](https://ubc-library-rc.github.io/gis-reference-mapping/content/hands-on5.html)r abridged like [Thematic mapping documentation. ](https://ubc-library-rc.github.io/gis-thematic-mapping/content/hands-on6.html) -->


### 1. Add the map
First things first, let’s add the map we made to our Print Layout. Click on “Add Map” from the Add Items menu. Your curser should turn into a crosshair when hovered over the page whitespace. Drag diagonally across your Print Layout page, corner to corner.


<img src="./images/layout7.png" style="width:100%">

> You might have to adjust symbol and text size accordingly in the Layer Properties of `public-baths` in the main QGIS interface. Once done, you can click the refresh icon in your Print Layout view and the print layout will update. Click save to save your work thus far. 
<img src="./images/refresh-icon.png" style="width:7%">



Once you add an item to your Print Layout, it will also show up in your **Items** list. The Items list is similar to your Layers Panel, but for the Print Layout. Click on any item in your Items list to view and modify its properties.



You’ll notice that Montreal might not take up the full page; in other words, it’s rather zoomed out. To zoom in, the most reliable method is simply to change its scale. We can do this from the **Item Properties**. You can activate an Item’s properties simply by clicking it in the Items list, and then looking at the Properties panel below it. Note: You’ll likely have to scroll to modify many of the properties, and resize your Items panel to reach the dropdowns.

item map properties picture


The scale number, `81153` in the demo screen, is the denominator in a fraction `1:81153`. This means 1 unit on the map represents `81,153`units in the real world. To zoom in, we want to reduce the denominator so that the fraction is a larger number, and 1 unit on the map corresponds to a smaller, more localized area in the real world. When in doubt, simply increase or decrease the scale number substantially to gauge which direction you need to go in. For this map, something like `45,000` should work.


<img src="./images/layout8.png" style="width:100%">

<img src="./images/layout9.png" style="width:100%">

<br>


- <img src="./images/move-content-icon.png" style="width:7%">
To move your map around within the frame itself, use the **Move item content** tool from the left-hand toolbar. 

- <img src="./images/select-content-icon.png" style="width:7%">
To select, resize, or move content like the map itself, use the **Move/Select item** tool.

<br>



### 2. Add a scalebar

Now that we've set the scale of our map, let's add a scalebar to the Print Layout. Just like above, you can add a scalebar from the **Add Item** menu at the top of your screen. (Remember, if you don't see this menu bar, make sure you're clicked into the Print Layout window.) Again, to add the scalebar item to your Print Layout, draw a small rectangle with your cursor. 


<img src="./images/layout9.png" style="width:100%">

Once you've added the scalebar, you can customize it. Choose a scalebar **Style** from the dropdown menu. The scalebar will adjust automatically if you adjust the scale of your map.

<img src="./images/layout10.png" style="width:100%">


Best practice is for your scale bar to be in **metric units**. 

To customize the symbology of your scalebar as well as its lettering, scroll down and expand the **Appearance** option. Click on **Font** in Appearance to change the font family and color of your scalebar labels. Thinking about Visual Hierarchy, perhaps the scalebar and lettering could be a lighter in color, or slightly transparent. Consider matching the lettering and line color with the water or other extensive features.  

<img src="./images/layout11.png" style="width:50%">


<br>

### 3. Add a north arrow

Add a north arrow. 

<img src="./images/layout12.png" style="width:100%">

If you scroll down to "Image Rotation" in Item Properties, you will notice there's an option to choose either Grid North or True North. Grid North is relative to the projection used, whereas True North, like the name implies, is a fixed geographic location. According to [QGIS](https://docs.qgis.org/3.40/en/docs/user_manual/print_composer/composer_items/composer_image.html), **Grid north** is the direction of a grid line which is parallel to the central meridian of the national/local grid, whereas **True north** is direction of a meridian of longitude. You can try changing - for the localization we're looking at it won't matter. 
<!-- There is also Magnetic North, which is Earth's magnetic pole and which shifts slightly. Depending on what projection is used and whereabouts your map is zoomed in to (near a pole or the equator; showing a large geographic area vs. a small one), which north orientation choose will be more or less important. Today's workshop won't go into the specifics, but Grid North is generally okay for maps not close to either poles and which cover a large area. [Read more on north arrows here](https://docs.os.uk/more-than-maps/geographic-data-visualisation/guide-to-cartography/north-arrows). -->
<!-- The [central meridian](https://gisgeography.com/central-meridian/) is where the 2-dimensional surface that's wrapped around the globe in a projection intersects with that globe. If your mapped area is around a central meridian, which is likely if you're using a UTM projection (in a specific Zone) or otherwise projection that's specifically designed for your region because of it's central meridian, then you can go ahead and use Grid North. If your map is centered on a region near the north (or south) pole, you might be better served using Truth North as that will angle the north arrow along the lines of longitude.  -->
{: .note}




### 4. Add a Title and Data Source.

Although you can add a title and other labels to your map based on layer attributes in the main QGIS interface, you can also add individual text labels, including place names as well as titles and attributes/data sources to the Print Layout via the Add Labels item. 

Go ahead and add a label for this map such as "Montreal's Historic Public Baths". To increase the font size and spacing, scroll down in the Item properties and click on Appearance. You can increase the spacing to stretch a title label across the extent of a feature. 

<img src="./images/layout13.png" style="width:100%">


You can up the size, font, and color by going to FONT under the Appearance option. 

<img src="./images/layout14.png" style="width:100%">

You can click over to add a buffer. My go to when color mapping for screen is a semi transparent buffer in the same color as the background. 

<img src="./images/layout15.png" style="width:100%">

<br><br>

At the bottom of your map, just above the neatline, it's customary to include the map author and data sources. This can be added as a label. The sources for this map are the City of Montreal and the Government of Canada, as well as Alex Alisauskas. 



Some notes on labelling: 
Visual Hierarchy is relevant to labelling in a couple ways. 
Color, transparency, size, yes
Also font style. 

All labels horizontal, with one exception for rivers and roadways which can follow shape of curve. 


<br>

### 5. Add a neatline

The border around your map frame is called a neatline. You can add a neatline by turning on the **Frame** option of your map item, and then styling it. Be sure to click back into your Map item in order to expose this item's properties. 

<img src="./images/layout16.png" style="width:100%">

Note - alighing map to horizontal and vertical center if need be. 

<br>



### 6. Legend
We don't need a legend here but if you were to add one, you'd add it from the Add Items menu. 

<img src="./images/layout17.png" style="width:100%">

Only features symbolized by your map should be included in your legend. Additionally, the names of relevant layers should be updated so they are understandable to the viewer.

To change the names or remove items from the legend, In the Legend Items section, collapse Main Properties so you can see Legend Items. Now, **uncheck the ‘Auto update’ box**. To remove any unnecessary layers, select the layer you want to remove and then click the big red minus sign. You may need to collapse the layer and scroll down. To rename a Legend item, simply double-click on the item and type in the text box that opens. Remember to click the back button to return to the the item properties. You can also go down to the background property and adjust transparency or remove altogether. 



<br><Br>
---

## Export your map
You can export your map as an image, PDF, or scalable vector graphic (`.svg`) from the Print Layout toolbar, or from the Layout menu. You can also print your map directly from QGIS. 

<img src="./images/export-map-icons.png" style="width:39%">
<img src="./images/layout20.png" style="width:100%">

When exporting as an image or PDF, you will be prompted to enter the resolution. I recommend increasing the resolution to at least 450dpi, otherwise your map will be blurry. 

**Congratulations! You've just made a map!**

Before you close your QGIS project, **save your Print Layout** and your Project too.







