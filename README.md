# World_Weather_Analysis

## Project Overview

The puporse of this analysis is to create a vacation map that allows users to choose according to weather criteria and identify their next travel destinations based on Temprature and Weather Conditions including:

1- A weather description to the pop-up markers for customers so that they know what the weather is as they are traveling.
2- A notation in the search criteria to indicate if it is raining or snowing for customers who are making travel decisions in real-time.
3- A map that shows the directions for customers’ travel itinerary.

By using Google API's we will also help the customers with ideal hotels suggestions within there preferred destinations.

## Resources

- Data sources: [weather_Database](/weather_Database/WeatherPy_Database.csv)
- Software : Python 3.7, Anaconda, Jupyter Notebook, Pandas.
- Google Maps API and Open Weather API keys.

## Summary 

In order to create the vacation map, we generated a list of 2,000 random latitudes and longitudes. With the coordinates, we retrieved and compiled a list of the nearest cities using the citipy module. Then, we used the OpenWeatherMap API to request the current weather data from each unique city on the list. The resulting map provides users with descriptions of the destinations found on our list, including: hotel name, city, country, and current weather and description. 
the map below shows the location of hotels oall over the world according to the weather preferrencies

![WeatherPy_vacation_map](/Vacation_search/WeatherPy_vacation_map.png)


- Once the customers have filtered the database (DataFrame) based on their temperature preferences, a heatmap will be showed to them for the maximum temperature for the filtered cities around the world.

![Vacation_search](/Vacation_search/WeatherPy_vacation_map.png)

A weather description to the pop-up markers will be displayed for customers so that they know what the weather is as they are traveling.

A map that shows the directions between multiple cities for customers’ travel itinerary will be displayed.

![Vacation_Itinerary](/Vacation_Itinerary/WeatherPy_travel_map.png)

A map that shows the directions between multiple cities with the details of the nearest hotel for customers’ travel itinerary will be also be displayed if selected by the customer.

![WeatherPy_travel_map_markers](/Vacation_Itinerary/WeatherPy_travel_map_markers.png)

