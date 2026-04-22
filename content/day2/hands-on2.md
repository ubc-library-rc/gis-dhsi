---
layout: default
title: 2. The Attribute Table
nav_order: 2
parent: Reference Mapping
---
# The Attribute Table
{: .no_toc}

Attribute table and selections!! 

Joins

Field Calculator

Edit Attribute Table too.... here... otherwise do more indept in the afternoon and just introduce as part of layer properties here,...

https://ubc-library-rc.github.io/gis-thematic-mapping/content/hands-on1.html


# The **Attribute Table**
The **Attribute Table** is where you can view the tabular data associated with vector datasets. Here, you can query your data by running complex selections, directly edit individual features, and perform mathematical operations on your layers. See the <a href="https://docs.qgis.org/3.40/en/docs/user_manual/working_with_vector/attribute_table.html" target="_blank">QGIS documentation on working with the attribute table</a> for more.


To open a layer's attribute table, right-click the layer in the Layers Panel and go to "Open Attribute Table". 

<img src="./images/table1.png" style="width:100%">


ALSO TOOLBAR TOOL


## Exploring the Attribute Table 


To Do
{: .label .label-green }
Open the attribute table of the `X` layer. 
Note that there are several attributes (columns) that describe each feature (row) in this dataset. Manually re-size the column widths until you can read each attribute.


The column headings are called **Attributes**. Each column is called a **Field** and each row is called a **Feature**. Each feature corresponds to one point on your map. (If you were looking at the attribute table of `vanHoods`, each feature would correspond to a polygon, and so on.) At the top of the Attribute Table you can see there are 3,224 features, or trees, in this dataset. Each feature, or tree, has 10 attributes, including the `common_name` and `height_m`. Notice that text values are left-justified whereas numerical values are right-justified. Sometimes cell values will be `NULL` meaning the feature contains no information for a given value. For instance, very few trees have information for the data planted. 

<img src="./images/table2.png" style="width:100%">


Notice that text values are left-justified whereas numerical values are right-justified. Sometimes QGIS will read numbers as text, disabling mathematical operations. If this happens, you will have to create a new field and set the type to either integer or decimal.

<br>

You can order Features in descending or ascending order by clicking on the attribute. 
- Click `height_m` to sort all Features from shortest to tallest. Click `height_m` again to sort from tallest to shortest. (Notice some of the shortest trees were planted just last month.) 
- Click `common_name` to sort the trees in alphabetical order. 

sort by occupation


<!-- *4*{: .circle .circle-yellow}
Form and Table view.  -->

## Selecting by Attribute
Selections are different than using the **Identify tool** to highlight a feature and expose its attributes. Selections select a set of features in the Attribute Table. Once attributes are thus selected, you can edit them, export them, or perform more analysis. 

There are many ways to make selections in QGIS. 
- You may **manually select** features from the map canvas using the **Selection Toolbar** <img src="./images/selections-toolbar.png" style="width:30%; display:inline">;
- You may **select features by location** using the **Select by location** vector analysis tool; 
- And you can **select features by attribute** within the Attribute Table. 


Other selections - we'll explore more in the afternoon. right now - select bakers from xyz.

or pick occupation

run selections for bakers from all 3 demographic layers, then from businesses to find bakeries??? 


To run a select by attribute... 

### Select bakers from x


we will use same skill to select religion? later on... and map by census tracts. or population density by ward or sensus tracts. 




