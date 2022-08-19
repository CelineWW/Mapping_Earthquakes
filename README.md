# Mapping_Earthquakes
## Overview
This project is aiming to create an earthquake map to visualize the earthquakes in past 7 days and major earthquake records around the world. Tectonic plates map was also added to reveal the reationship between earthquakes and plates. 

1. Using street map and satellite map as base layer, map all recorded earthquakes in the past 7 days. Add some features to the map to showcase the severity of earthquakes for viewers
2. Add tectonic plate data and major earthquake data to the map using d3.json(). 
3. Add color and set the radius of the circle markers based on the magnitude of earthquake. Add a popup marker for each earthquake that displays the magnitude and location of the earthquake using geoJSON().
4. Add a dark map style as a tile layer object.


## Result

 - Add street map and satellite map as base layer option
    
 - Map all earthquakes with Point geoJSON data as an overlay map. 
   
   Circle marker colors and radius were styled to appeal viewers based on the magtitude of earthquakes.
   A legend was created on the bottom right to show magnitude range.
   Popups show more details about Magnitude and location. 
  
    ![all earthquakes](https://user-images.githubusercontent.com/105877888/185702702-114d3fb8-b2e0-41a6-b5d8-831f4c308fd5.png)

      
    ![satellite map](https://user-images.githubusercontent.com/105877888/185682085-4330921d-a072-4826-802a-14a98b56552b.png)

 - Map tectonic plates with LineString geoJSON data as an overlay map
  
    ![tectonic plates](https://user-images.githubusercontent.com/105877888/185681411-c372c3f7-03f5-4e2f-a0db-98b592d8573e.png)

  
 - Map major earthquakes with Point geoJSON data as an overlay map
  
    ![major earthquakes](https://user-images.githubusercontent.com/105877888/185681433-541feed2-8a51-40a0-8210-d871101bbfa7.png)

 - Add dark map tile layer to base map option

    ![darke  map](https://user-images.githubusercontent.com/105877888/185682220-0d2ce2da-b24f-4321-9f15-67c5074ab79b.png)


## Summary
Overall, the webpage looks nice. The contents are coherent. Multi-filter works functionally. The theme and background image match the UFOs content very well. Still, the webpage can be improved a little bit. 
  1. A drawback of this webpage
     
     The data source is limited. The observation record of UFOs only covers the date from 1/1/2020 through 1/13/2020. This is unsufficient for this webpage. More data need to be collected. If it is impossible to get more date, there should be a remark beside `Enter Date` filter to clarify the date period.
  
  2. Two additional recommendations for further development 
     
     1. The text `Filter Search` is very frustrating for the users. It looks like a filter button, quite misleading. At the same time,  `UFO Sightings` button which is for unfiltering is on the very top left corner. Users might not notice it. For further improvement, I would suggest to create two buttons: `Filter Search` and `Go Back` below multi-filters. `Filter Search` button will triger the filter to show the filter results after user input the filters and click the `Filter Search` button. Whereas `Go Back` will take over the function of `UFO Sightings` button. It will guide user to go back to unfiltered table.
     2. The filter input must be exact macth to the format of data value in database. Currently, the input of city, state, country must be lowercase. Even though there are examples for each filter, these are not popular format for common use. If we can add a couple of codes to igonre or convert all input uppercase letter to lowercase letter, it will provide users a better experience on searching.
     
