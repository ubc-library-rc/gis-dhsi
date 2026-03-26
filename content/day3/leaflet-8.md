---
layout: default
title: 8. Clustering
nav_order: 8
parent: Hands on with Leaflet
---
# Clustering a point layer
Clustering aggregates point data for certain zoom levels, generalizing otherwise busy maps. As you zoom in, clustered data points will disperse, adding specificity. 

<iframe src="./reference/art-and-heritage-clustered.html" style="width:100%; height:520px; border:none;"> </iframe>

Rather than devise the code to cluster a dataset yourself, all you need to do is add some additional code libraries to your map. While you could download the [Leaflet.markercluster plugin](http://leaflet.github.io/Leaflet.markercluster/) directly to your computer/workshop data folder and link it locally just like you link your datasets, it's far easier to simply link the relevant libraries in the `<head>` element of your map HTML document. Remember, this is how we powered our map with Leaflet to begin with.
<!-- https://github.com/Leaflet/Leaflet.markercluster -->

After adding the **Leaflet.markercluster** libraries, we will then use this function to cluster our dataset.

----


## Add `Leaflet.markercluster`
At the very bottom of the `<head>` element, add the following. Be sure to scroll-right to get all of it. 

```html
  <!--marker cluster libraries-->
  <link rel="stylesheet" href="https://unpkg.com/leaflet.markercluster@1.4.1/dist/MarkerCluster.css">
  <script src='https://unpkg.com/leaflet.markercluster@1.4.1/dist/leaflet.markercluster-src.js'></script>
  <link rel="stylesheet" href="https://unpkg.com/leaflet.markercluster@1.4.1/dist/MarkerCluster.Default.css" />
```
<br>

## Add point layer as cluster group
In the `<script>` element of your map's `<body>`, locate the codeblock that adds and loads Public Art as a point layer.  Either delete this block, or, more preferably, comment it out. In its place, copy and paste the following code. 


```js
//  add art layer as cluster group 
    var markers = L.markerClusterGroup();

    L.geoJSON(art, {
      onEachFeature: function (feature, layer) {
        var popupContent =
          "<img src='" + feature.properties.ImageURL + 
          "' width='200px'/><br><b>Title: </b>" + 
          feature.properties.Title + 
          "<br><b>Artist: </b>" + 
          feature.properties.Artist
        layer.bindPopup(popupContent);
      },
    }).addTo(markers);
    markers.addTo(mymap);
```

<br>

That's it! Your point layer should now be clustered. 