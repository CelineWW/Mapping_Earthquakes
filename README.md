# Mapping_Earthquakes
## Overview

This project is focusing on developing a dynamic webpage by inserting JavaScript data source into an HTML page. 
1. Build a table to hold and display UFO observation data.
2. Add a filter to take user inputs and adjust the table accordingly through multi-filter. 
3. Insert the table into a well-structured HTML page.
4. Use bootstrap and css to style the webpage.
5. Add title and an article to webpage as a brief introduction for the analysis background.

## Result

This dynamic webpage can be explored by doing following steps:
  - Open the webpage by clicking index.html
  - Browse the title, summary article, and table columns.
  
  
  - Add street map base layer
    

  - Map all earthquakes with Point geoJSON data
  
    ![all earthquakes](https://user-images.githubusercontent.com/105877888/185680453-d4ae4216-7ed8-43a1-930c-78e0c7aa422d.png)
    
  - Add satellite map
  
    ![satellite map](https://user-images.githubusercontent.com/105877888/185682085-4330921d-a072-4826-802a-14a98b56552b.png)

  - Map tectonic plates with LineString geoJSON data 
  
    ![tectonic plates](https://user-images.githubusercontent.com/105877888/185681411-c372c3f7-03f5-4e2f-a0db-98b592d8573e.png)

  
  - Map major earthquakes with Point geoJSON data
  
    ![major earthquakes](https://user-images.githubusercontent.com/105877888/185681433-541feed2-8a51-40a0-8210-d871101bbfa7.png)

  - Add dark Map tile layer 

    ![darke  map](https://user-images.githubusercontent.com/105877888/185682220-0d2ce2da-b24f-4321-9f15-67c5074ab79b.png)


*An example multi-filter and its result:*
```
Enter Date : 1/1/2010
Enter a City: ----
Enter a State: ----
Enter a Country: us
Enter a Shape: sphere
```


## Summary
Overall, the webpage looks nice. The contents are coherent. Multi-filter works functionally. The theme and background image match the UFOs content very well. Still, the webpage can be improved a little bit. 
  1. A drawback of this webpage
     
     The data source is limited. The observation record of UFOs only covers the date from 1/1/2020 through 1/13/2020. This is unsufficient for this webpage. More data need to be collected. If it is impossible to get more date, there should be a remark beside `Enter Date` filter to clarify the date period.
  
  2. Two additional recommendations for further development 
     
     1. The text `Filter Search` is very frustrating for the users. It looks like a filter button, quite misleading. At the same time,  `UFO Sightings` button which is for unfiltering is on the very top left corner. Users might not notice it. For further improvement, I would suggest to create two buttons: `Filter Search` and `Go Back` below multi-filters. `Filter Search` button will triger the filter to show the filter results after user input the filters and click the `Filter Search` button. Whereas `Go Back` will take over the function of `UFO Sightings` button. It will guide user to go back to unfiltered table.
     2. The filter input must be exact macth to the format of data value in database. Currently, the input of city, state, country must be lowercase. Even though there are examples for each filter, these are not popular format for common use. If we can add a couple of codes to igonre or convert all input uppercase letter to lowercase letter, it will provide users a better experience on searching.
     
