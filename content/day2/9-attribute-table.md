---
layout: default
title: 1. The Attribute Table
nav_order: 1
parent: Thematic Mapping
---
# The Attribute Table
{: .no_toc}

The **Attribute Table** is where you can view the tabular data associated with vector datasets. Here, you can query your data by running complex selections, directly edit individual features, and perform mathematical operations on your layers. See the [QGIS documentation on working with the attribute table](https://docs.qgis.org/3.40/en/docs/user_manual/working_with_vector/attribute_table.html) for more.

<details open markdown="block">
  <summary>
    On this page:
  </summary>
  {: .text-delta }
 - TOC
{:toc}
</details>
----

## Exploring the Attribute Table 
If you haven't already, launch the `thematic-mapping.qgz` project in the folder `dhsi-workshop/Day2/thematic-mapping`. Turn on the layer `census1881`. 

<img src="./images/table1.png" style="width:100%">

<br>

- To open a layer's attribute table, right-click the layer in the Layers Panel and go to "Open Attribute Table". 

<img src="./images/table2.png" style="width:100%">

You can also use the Attributes Toolbar (so long as it's turned on) to open the Attribute Table of a layer highlighted in the Layers Panel. 
<img src="./images/table2b.png" style="width:7%">

The attribute table might take a while to load as there are over a hundred thousand points. Additionally, since the attribute table will open in a new window, sometimes this can get lost behind the main QGIS interface. 

<br>

Note that there are several attributes (columns) that describe each feature (row) in this dataset. Manually re-size the column widths until you can read each attribute.


<img src="./images/table3.png" style="width:90%">

<br>
The column headings are called **Attributes**. Each column is called a **Field** and each row is called a **Feature**. Each feature corresponds to one point on your map. (If you were looking at the attribute table of `vanHoods`, each feature would correspond to a polygon, and so on.) At the top of the Attribute Table you can see there are 111,208 features, or census returns, in this dataset. Each feature, or person, has multiple attributes, including the `NOM_NAME` and `AGE`, `OCCUPATION` and `RELIGION`. Sometimes cell values will be `NULL` meaning the feature contains no information for a given value. For instance, not all individuals entered an occupation. 



Notice that text values are left-justified whereas numerical values are right-justified. Sometimes QGIS will read numbers as text, disabling mathematical operations. If this happens, you will have to create a new field and set the type to either integer or decimal.
{: .note}

<br>


You can order Features in descending or ascending order by clicking on the attribute. 
- Click `AGE` to sort all Features from youngest to oldest. (Null will appear first; scroll past these to reach infants.) Click `AGE` again to sort from tallest to shortest. 
- Click `OCCUPATION` to sort the trees in alphabetical order. 

On the bottom-right hand corner there are two icons allowing you to toggle between "Table View" (your current view) and "Form View". Form view will show you a summary of all a feature's attributes. 

<img src="./images/table4.png" style="width:10%">


<br>

At the top of the Attribute Table you'll see some tools. Let's take a closer look at these now. 

<img src="./images/table5.png" style="width:100%">

<br>


## Selecting by Attribute
Selections are different than using the **Identify tool** to highlight a feature and expose its attributes. Selections select a set of features in the Attribute Table. Once attributes are thus selected, you can edit them, export them, or perform more analysis. 

There are many ways to make selections in QGIS. 
- You may **manually select** features from the map canvas using the **Selection Toolbar** <img src="./images/selection-attribute-toolbar.png" style="width:30%; display:inline">;
- You may **select features by location** using the **Select by location** vector analysis tool; 
- And you can **select features by attribute** within the Attribute Table. 


<!-- Other selections - we'll explore more in the afternoon. right now - select bakers from xyz. -->

<!-- or pick occupation

run selections for bakers from all 3 demographic layers, then from businesses to find bakeries???  -->


We will be using historic data for Montreal to visualize the spatial distribution and density of French Canadians according to the 1881 census. So, we want to select just those identified as French Canadian from this dataset. There are a couple different ways we could run this query: we could select all individuals who have an origin listed as French (and derivatives such as xyz), or we could select those whose ethnicity `ETH` is french canadian (`FC` or `fc`). To make our lives simpler we will do the latter. 


*1*{: .circle .circle-yellow} From the Attribute Table of `census1881`, click on the **Select features using an expression** button.

<img src="./images/table6.png" style="width:100%">


We will use this tool to query and select only features where `ETH` is “FC” or `ETH` is “fc” . Rather than writing an expression by hand, we will select the appropriate fields, values, and operators from the drop-downs provided. This ensures no syntax errors are made and our selection runs smoothly.


*2*{: .circle .circle-yellow} From the middle panel, expand **Fields and Values**. Double click on `ETH` to add it to the Expression builder.

<img src="./images/table7.png" style="width:80%">
<br>

*3*{: .circle .circle-yellow} Then click the `=` operator. You will get a warning saying your expression is invalid. That's okay! We aren't finished building it.

<img src="./images/table8.png" style="width:80%">

<br>

*4*{: .circle .circle-yellow} Finally, we need to indicate what Ethnicity is equal to. In the right-hand panel, click the button for **All Unique** to display all the unique values for common name in the dataset. This is a handy way to find out the unique values of any given attribute. 

French Canadian is abbreviated to FC. However, *it is both upper case and lower case*. We have to include both. 

First, double-click on "FC" to add it to the expression. Then, add the text `or`, and add `ETH` `=` again. Then double-click "fc". **Your final expression should now be ` "ETH"  =  'FC' or  "ETH"  =   'fc'`.** IT IS VERY IMPORTANT YOUR EXPRESSION MATCHES EXACTLY.

<img src="./images/table9.png" style="width:80%">

<br>
*5*{: .circle .circle-yellow} Now click **Select Features** on the bottom-right. Close the expression builder and return to the Attribute table. You will see that 59,033 features have been selected. Selected features will be highlighted in the Attribute Table. If you the Attribute Table indicates a selection was made but you don't see any highlighted features, try ordering the Attribute Table by `ETH`, and then scrolling down to the letter "F". 

<img src="./images/table10.png" style="width:90%">

<br>
Note: You can also choose to Show Selected Features only. Alternatively, you can change the Attribute Table view to view *only selected features*. Just be sure to change the view back afterwords, or next time you open the attribute table it will appear empty if no selections have been made.  

<img src="./images/table11.png" style="width:40%">

<br>

Close the Attribute Table and return to the main QGIS interface. In the Map View, you should see your selection highlighted. Now that you've selected only individual's whose ethnicity is French Canadian, we can export this selecten as a brand new dataset. 


<img src="./images/table12.png" style="width:90%">

<br>

*6*{: .circle .circle-yellow}
Right-click on the layer `census1881` in the Layers Panel. Choose **Export** and then be sure to choose **Save *selected* Features As**. 

<img src="./images/table13.png" style="width:100%">

<br>


*7*{: .circle .circle-yellow} In the window that opens, give the new file both a name *and a location*. To give it a location, click on the three dots and navigate to the `dhsi-workshop/Day2/thematic-mapping` folder. Call this file `french-canadians`. 

- Keep it an Esri Shapefile. 
- Keep the projection set to the Project CRS. 

<!-- **Then, expand "Select fields to export and their export options". Scroll down to `geo_point_2d` and check `Use Key/Value`.** -->


Click Okay. The new layer should be created and automatically added with a new default color to your map. If not, add it now. 


<img src="./images/table14.png" style="width:100%">

<br>

**Save your project**. 

<br>

## Count points in polygon 
Since our goal is to create a thematic map that visualize the spatial distribution of French Canadians in historic Montreal, we need to find out how many French Canadians filled out a census in each census tract.  While we could count up the many, *many* points by hand, this would take a long time and could introduce human error. Instead, we will use QGIS vector analysis tools to do the counting for us. 

Tomorrow we will go into more detail about tools and workflows in QGIS. Today we will use 2 tools: count points in polygon and centroids to xyz. 

Processing Toolbox. 
There are two main ways to access spatial analysis tools in QGIS: 1. through the **Vector** menu and 2. through the **Toolbox** located in the **Processing** menu.

Go ahead and open the **Processing Toolbox**. 


If you don't see the **Processing** menu at the top of your screen, you may have to enable the processing plugin. Click on the **Plugins** menu at the top of your screen, and then on **Manage and Install Plugins…**. In the search bar, type in "Processing". Make sure to **select the Processing box**, and then click Close. You should now see the Toolbox icon and be able to proceed with the next steps. Once enabled, you will be able to access the Processing menu anytime you open this or any other QGIS project. 
{: .note} 




In the Processing Toolbox, search for the QGIS tool called **Count points in polygons**. It will be nested under **Vector analysis**. This tool will count the number of points (French Canadians) in each polygon (Historic Montreal census tracts), and append the total to each census tract in `census_tracts` as a new attribute. 


*1*{: .circle .circle-yellow} In the tool window, select the following inputs:

- **Polygons**: `census_tracts` 
- **Points**: `french-canadians` 
- **Count field name**: `FC` (the name of the attribute that will store the total French Canadians for each census tract.)


<img src="./images/" style="width:100%">


Click **Run**, then **Close** when the process has finished. Note: you may see the caution ‘No spatial index exists for points layer, performance will be severely degraded’. You can ignore this.


*You should now have a new layer called `Count` in your Layers Menu*. This is because, unless you specify the output of a tool to be a permanent layer, it will create a temporary layer with the tool's name. 

<br>
*2*{: .circle .circle-yellow} Drag `Count` below `census_tracts` in Layers Panel so the distribution of Douglas Firs remains visible on your Map Canvas. Take a look at the Attribute Table for `Count`. You can now see the number of French Canadians in each census  tract. Close the attribute table to continue.


<img src="./images/" style="width:100%">

<br>

*3*{: .circle .circle-yellow} Save `Count` as a permanent layer to your data folder by right-clicking it and selecting either **Make Permanent** or **Export - Save Features As..**. Save the file to the `dhsi-workshop/Day2/thematic-mapping/` folder and call it `french-canadians-count`. Everything else can remain as default. Click **OK**. Note that if you have any trouble exporting the file, it's likely because you didn't specify a location, just a name for it. 

<br>

*4*{: .circle .circle-yellow} Be sure to add `french-canadians-count` to your project if it doesn't add automatically. Then, remove `Count` and **Save your project**. 


RUN THE SAME WORKFLOW TO APPEND TOTAL POPULATION PER CENSUS COUNT TO CENSUS TRACTS. 
<!-- ## Centroids: From polygon to point  -->

<!-- run centroid on count (for proportional symbol map later) or move to proportional symbol map section 

wait no do later - all as part of prop. symbol mapp activity
-->



<br> 

## Joins 

join total-pop-count to french-canadian-count. 

show how to. 


<br>


## Field Calculator 






## workflow ... 

Percentage French Canadian Workflow... 

select and export attribute where eth = FC or fc. 

save as.


count points in census tract polygon both for french-canadian and for total population. 

join count for total pop to count for french-canadian-count. 

then show how to edit attributetable, field calculator to make new column thats percent. 

then next page - choropleth map. 




