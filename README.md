# Mapping_Earthquakes
## Overview
This project is aiming to create an earthquake map to visualize all earthquakes and major earthquakes in past 7 days around the world, and trying to discover the realtionship between tectonic plates and earthquakes. 

1. Using street map and satellite map as base layer, map all earthquakes data in the past 7 days. Add some features to the map to show the severity of earthquakes for viewers.
2. Add tectonic plate data and major earthquake data to the map using d3.json(). 
3. Add color and set the radius of the circle markers based on the magnitude of earthquake. Add a popup marker for each earthquake that displays the magnitude and location of the earthquake using geoJSON().
4. Add a dark map as an additional tile layer.


## Result

 - Use street map and satellite map as base layer options, map all past 7 days earthquakes with Point geoJSON data as an overlay. 
   - Circle marker colors and radius were styled to appeal viewers based on the magtitude of earthquakes.
   - A legend was created on the bottom right to show magnitude range.
   - Popups show more details about Magnitude and location. 
  
    ![all earthquakes](https://user-images.githubusercontent.com/105877888/185702702-114d3fb8-b2e0-41a6-b5d8-831f4c308fd5.png)

      
    ![satellite map](https://user-images.githubusercontent.com/105877888/185682085-4330921d-a072-4826-802a-14a98b56552b.png)

 - Map tectonic plates with LineString geoJSON data as an overlay
  
    ![tectonic plates](https://user-images.githubusercontent.com/105877888/185681411-c372c3f7-03f5-4e2f-a0db-98b592d8573e.png)

  
 - Map major earthquakes with Point geoJSON data as an overlay
  
    ![major earthquakes](https://user-images.githubusercontent.com/105877888/185681433-541feed2-8a51-40a0-8210-d871101bbfa7.png)

 - Add dark map tile layer to base map options

    ![dark map](https://user-images.githubusercontent.com/105877888/185706886-5520fce6-0997-4fff-bdab-1f00f5e16bf9.png)

## Summary
- Three map styles: `Streets, Satellite, Dark` were provided as base map options. All earthquakes and major erathquakes data in past 7 days and tectonic plates data were all added to the map, which can be folded up. 
- From the view of earthquake locations and tectonic plate boundaries, Major earthquaks mainly happen on or close to plate boundaries.
- Still, there are a couple of drawbacks for the project.
  1. Since geologic movement is dynamic, earthquake status changes every minute. The geoJSON file we used for mapping here is static. It is better to choose a real-time earthquake link to get most updated information.
  2. Popups only include magnitude and location of individual earthquake. The Date and time when earthquake happened is another parameter that Viewers may concern. It should be added to popups too.
   
