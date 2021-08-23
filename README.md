# World_Weather_Analysis
## Overview
Create additional functionality to a theoretical app- PlanMyTrip.  The new functions will allow users to plan a trip itinerary based on maximum and minimum temperatures to help identify cities and hotels that meet those requirements.  Using mapping tools, a visualization via google maps will show the user the cities and hotels for their trip, along with driving directions.  

## Source Data
  - cities.csv
  - OpenWeatherMap
  - gmaps

## Software Used
   - Jupyter Notebook
   - Python 3.6
   - Pandas
## Process
Using citipy module in jupyter notebook, the nearest city to over 2000 randomly generated latitudes and longitudes was retrieved.  An API call is made to OpenWeatherMap to retrieve location and weather information about the city.   

![apicall](https://user-images.githubusercontent.com/79231355/130525109-76ff78bf-028f-41de-b3b9-8b7e247475a7.png)

The retrieved data is parsed and added to a data frame.

![parse_1](https://user-images.githubusercontent.com/79231355/130525119-fe6f2f87-df37-4fde-a0b3-2d0cc255a6ec.png)
![parse_2](https://user-images.githubusercontent.com/79231355/130525126-beb32812-4030-47dc-b8d7-e40f920cd459.png)

Weather data is loaded into a new notebook where users must enter the maximum and minimum temperature for their desired trip.  

![tempentry](https://user-images.githubusercontent.com/79231355/130525142-1f5e0d16-51ad-4480-8e54-84f4a58286ef.png)

The cities are filtered based on the entered information.

![dataframe](https://user-images.githubusercontent.com/79231355/130525284-38e5da2d-b2ff-43af-a105-2fc752e20045.png)

![WeatherPy_vacation_map](https://user-images.githubusercontent.com/79231355/130525333-c1c101ba-b6c8-46d9-9f13-b910e7cb2b32.png)

An API call is made to gmaps to locate hotels close to the latitude and longitude from the citipy weather response and added to a new column in the data frame.  

![hotels](https://user-images.githubusercontent.com/79231355/130525260-a95c954e-fae8-46c9-84a6-d08896a5ae89.png)

Hotel names are added to pop up markers on a map. 

![hotel_marker](https://user-images.githubusercontent.com/79231355/130525293-a0fe80d3-9fe5-42ec-a697-65531a1f60ee.png)

![WeatherPy_travel_map_markers](https://user-images.githubusercontent.com/79231355/130525357-526ef883-bbc0-4d67-a8ce-99f20b82aa3d.png)

 The hotel and weather information is then used to generate a 4 city itinerary of travel.   
 
 ![itenerary](https://user-images.githubusercontent.com/79231355/130525300-badab636-d244-4f6b-8433-75b317f9ae4d.png)
 
 ![WeatherPy_travel_map](https://user-images.githubusercontent.com/79231355/130525376-9dd0ef94-3a03-4ffb-a6ca-ff612fb35bba.png)

# Results
The new functions of the app work as intended.  Users are able to input a desired temperature range and over 2000 cities are parsed through OpenWeatherMap that need that criterion.  Gmaps is used to find nearby hotels.  Gmaps also displays them visually using google maps with information available by selecting a balloon over the hotel.  Users select their desired hotels for their trip itinerary.  Gmaps then maps the driving directions and displays the selected hotels on google maps with the additional information above each hotel that was previously selected in the itinerary.  

The application is still limited in that only the closest hotel is displayed to the listed city coordinates.  Additional variety could be added for the user if additional hotels were available, or criteria was able to be entered for the type or class of hotel.  Also, the city names are somewhat limited due to the limitation placed on the number of cities available from the OpenWeatherMap Search.  Adding additional criteria after the initial search so that users could select regions, and then search again, to produce additional cities for selection could increase user satisfaction with the app.
