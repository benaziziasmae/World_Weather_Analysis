# World_Weather_Analysis

## Project Overview

The puporse of this analysis is to create a vacation map that allows users to choose according to weather criteria and identify their next travel destinations based on Temprature and Weather Conditions including:

1- A weather description to the pop-up markers for customers so that they know what the weather is as they are traveling.

2- A notation in the search criteria to indicate if it is raining or snowing for customers who are making travel decisions in real-time.

3- A map that shows the directions for customers’ travel itinerary.

By using Google API's we will also help the customers with ideal hotels suggestions within there preferred destinations.

- There are three folders here that offer different levels of analysis: weather database, vacation search, and vacation itinerary.(let's break them down._

## Resources

- Data sources: [weather_Database](/weather_Database/WeatherPy_Database.csv)
- Software : Python 3.7, Anaconda, Jupyter Notebook, Pandas.
- Google Maps API and Open Weather API keys.

# Summary 

## Deliverable 1

In order to create the vacation map, we generated a list of 2,000 random latitudes and longitudes. With the coordinates, we retrieved and compiled a list of the nearest cities using the citipy module and perform an API call with the OpenWeatherMap. Then, we used the OpenWeatherMap API to request the current weather data from each unique city on the list. The resulting map provides users with descriptions of the destinations found on our list, including: hotel name, city, country, and current weather and description. 

We generate the following database:

**WeatherPy_Database**

This folder uses Open Weather Map API to pull weather information on over 700 different cities around the world. That information consists of:

- Maximum Temperature
- Cloudiness
- Wind Speed
- Humidity
- Current Weather Description

These different categories of information make it easy for travelers to choose exactly what they are looking for in a travel destination.

[WeatherPy_Database](/weather_Database/WeatherPy_Database.csv)

## Deliverable 2

In order to create a user travel map, we had to retrieve customer weather preferences, then use those preferences to identify potential travel destinations and nearby hotels. Then, show those destinations on a marker layer map with pop-up markers.

We take the information gained in the weather database and uses Google Maps API to plot different travel destinations with a hotel at each location. The image below shows the locations of all the places in the database that have an daily maximum temperature between 75 and 90 degrees farinheit.

The map below shows the location of hotels around the world according to the weather preferrencies.

![WeatherPy_vacation_map](/Vacation_search/WeatherPy_vacation_map.png)

## Deliverable 3

In order to create a user travel itenerary map, wa had to use the Google Directions API to create a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations. Then, create a marker layer map with a pop-up marker for each city on the itinerary.

Then we take the search information from the search folder and uses Google Maps *Directions API* to create a vacation itinerary. For example, the map below shows a 4 stop itinerary in **Mexico** that features  Tomatlan, Lazaro Cardenas,Fresnillo, and San Blas to arrive finally to Cabo San Lucas.

![Vacation_Itinerary](/Vacation_Itinerary/WeatherPy_travel_map.png)

A map that shows the directions between multiple cities with the details of the nearest hotel for customers’ travel itinerary will be also be displayed if selected by the customer.

![WeatherPy_travel_map_markers](/Vacation_Itinerary/WeatherPy_travel_map_markers.png)


