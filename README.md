# Mapping_Earthquakes

## Overview
The purpose of this project was to utilize GeoJSON data from github to develop interactive maps using HTML and JavaScript to display earthquake data from across the world.  Maps were using JavaScript to display points. lines, varying layers, and adding specifications to the layers to display certain characteristics such as the radius.  D3 was also used edit the style of our maps and make it much more visually appearling.  The final product was an interactive map displaying major earthquakes from around the world based on their 
magnitude and displaying fault lines.

## Resources
GeoJSON resources: 
  - https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_week.geojson
  - https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/4.5_week.geojson
  - https://raw.githubusercontent.com/fraxen/tectonicplates/master/GeoJSON/PB2002_boundaries.json

## Tools Used
  - CSS 
  - HTML 
  - D3 
  - JavaScript
  - Leaflet

## Results

### 1. Adding Layers
A second layer group was added to display tectonic plate data and referenced using d3.  The layer was edited to contain colors and weights and added to the map.  The map displayed the ability to select Satellite or Streets view, and Tectonic Plates and Earthquakes as options to view.
![image](https://user-images.githubusercontent.com/88444529/153428208-0e3bd594-9c68-445f-967e-738fcbdcf115.png)
![image](https://user-images.githubusercontent.com/88444529/153428702-b7f88582-1af9-404f-ac12-6bb9442aeb89.png)

### 2. Displaying Major Earthquake Data
Major earthquake data was then added to the map by adding a third layer group that overlay object.  By using the d3 callback method a call was made to the GEOJson summary feed for major earthquakes hapenning over the last 7 days.  By using the parameters in the StyleInfo, the color and radius were added under the condition of magnitude of earthquake that is either greater than 5, greater than 6, and less than 5.  This was all added to the map and displayed as follows.
![image](https://user-images.githubusercontent.com/88444529/153430556-5a04b62f-10ca-4d25-b22b-b112fe345c0d.png)

### 3. Dark Map Added 
Finally, using JavaScript and leaflet.js an addition map was added.  A map was added that was "dark" and is able to be selected.
![image](https://user-images.githubusercontent.com/88444529/153430983-8d213389-1fca-4ea9-b85c-8e86d55f1139.png)

## Conclusion
Other layers and maps were successfully added to our original map that displayed tectonic plate data, major earthquake data, and an additional map type.  This was all done by editing the HTML code, utilizing JavaScript and leaflet.js, and inspecting the GeoJSON code.  Overall, this map is interative and displays the information as it is supposed to.  In the future, additional features can be added and taken away as needed.

## Contact Information

danjoyce6@gmail.com
