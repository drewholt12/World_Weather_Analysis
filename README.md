# World_Weather_Analysis
Create additional functinonality to a theoretical app- PlanMyTrip.  The new functions will allow users to plan a trip itenerary based on maximum and minimum temperatures to help identify citys and hotels that meet those requirements.  Using mapping tools, a visualization via google maps will show the user the cities and hotels for their trip, along with driving directions.  

## Source Data
  - cities.csv
  - OpenWeatherMap
  - gmaps

## Software Used
   - Jupyter Notebook
   - Python 3.6
   - Pandas

# Results
The new functions of the app work as intended.  Users are able to input a desired temperature range and over 2000 cities are parsed through OpenWeatherMap that need that criteria.  Gmaps is used to find nearby hotels.  Gmaps also displays them visually using google maps with information available by selecting a balloon over the hotel.  Users select their desired hotels for their trip itinerary.  Gmaps then maps the driving directions and displays the selected hotels on google maps with the additional information above each hotel that was previously selected in the itinerary.  

The application is still limited in that only the closest hotel is displayed to the listed city coordinates.  Additional variety could be added for the user if additional hotels were available, or criteria was able to be entered for the type or class of hotel.  Also, the city names are somewhat limited due to the limitation placed on the number of cities available from the OpenWeatherMap Search.  Adding additional criteria after the initial search so that users could select regions, and then search again, to produce additional cities for selection could increase user satisfaction with the app.
