# Mapping_Earthquakes

#### Overview
The goal of this project was to create a web page that could clearly and effectively present the locations and magnitudes of recent earthquakes around the globe. The data were provided in GeoJSON formats from the following URLs: https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_month.geojson, https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/4.5_week.geojson, https://raw.githubusercontent.com/fraxen/tectonicplates/master/GeoJSON/PB2002_plates.json. Of course, the code files that refer to these web pages contain attributions as well. To style the web page, I used the styles provided by Mapbox. 

#### Methods
The first step was to use HTML to get the web page started and to consider the general design of this page. In this case, I wanted it to be simple and straightforward, so the page immediately opens with a general map of Earth. From there, the user can select the different styles to view and overlays to select. This is done by incorporating Leaflet's style options for displaying different types of elements and layers. These include point markers, lines between points, and polygons to represent various areas or borders. In JavaScript, I first created the tile layers that I would use to display the data on the map. I then linked the map object to the id tag in the HTML script and included the latitude and longitude coordinates to center the map. Next, creating a base maps layer that accessed the different map styles would allow the user to choose between them when using the web page. Ultimately, the D3 and Leafelet packages for JavaScript allowed me to parse the GeoJSON data and extract the data I needed for this project. 

#### Results

![Earthquake Map in Action](https://raw.githubusercontent.com/veachk90/Mapping_Earthquakes/main/Screenshot%20(185).png)

Pretty cool, huh? At this point, the web page and the data presented are relatively simple. However, with this initial project done, there are many addenda that could be made from the data contained in the GeoJSON sources. It could also be interesting to incorporate data that may not be readily available in the sources already used, such as the damage caused by each earthquake. 
