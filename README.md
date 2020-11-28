# WeatherPy Analysis

This is an analysis for any traveller with three particular endpoints:

 - Retrieve current weather data for a handful of locations;
 - Filter from those locations based on the customers' temperature preference and show a map of the filtered locations;
 - Pick four random cities and show a travel map with popular transport modes (Driving, Walking or Bicycles) 

## Analysis
The analysis starts with generating a random list of coordinates to retrieve the location data & current weather for them. This included subscribing to the Citipy python module as well as the Openweathermaps API. This allowed to retrieved the city name with the Citypy module and then retrieving their current wether via the Openweathermaps API.

Once the weather was retrieved, the locations were further filtered to find out locations based on the customer's / traveller's temperature preference. This saved the filtered locations list separately and then showed a map of the locations with markers about some general information about each location. This included subscribing to Google's Maps API.

Finally, four random cities were picked in a single country and a travel route was shown on top of the map generated based on the traveller's preference. Popular travel methods used are driving, biking or walking. Google's Directions API was used for this purpose.

## Results and afterthought

This is a pretty simple search template for a traveller to go through and pick a location for travel purpose. This allows for them to pick a single country and check through the travel modes for different cities. This can be modified to include cross country travel as well.

## Dependencies

Dependencies for this module are as follows:
    
    - Python
    - Subscription to Google API platform
    - Subscription to OpenweatherMaps API platform