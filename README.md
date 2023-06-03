# Weather
This is my personal favourite! The sole aim is to identify cities within a radius of a home city where the weather conditions are perfect to enjoy your next planned vacation!
For this project, I haved used geonames which provides a free tier for their APIs, for weather I have used open-meteo- which again is a free service and doesn't require username/authentication.

The Weather class:

Provides weather forecasts using the Open-Meteo API.
Supports fetching daily and hourly weather attributes for a specified number of days.
Implements a caching mechanism for storing weather data to avoid unnecessary API calls.
Allows analysis of weather data, including calculating averages and combining daily and hourly data.
The Findme class:

Retrieves nearby cities based on a specified radius and city type using the Geonames API.
Implements caching to store the results of nearby cities to avoid redundant API calls.
The bulk_weather method:

Collects weather data for all nearby cities.
Allows customization of thresholds for precipitation, temperature, and cloud cover.
Utilizes the Weather class to fetch weather data and perform analysis.
The bulk_fetch method:

Filters the weather data based on predefined conditions (sunny or cloudy).
Constructs a dictionary containing city names, coordinates, and weather conditions.
The bulk_plot method:

Generates an interactive map using the folium library.
Adds markers for each city on the map, indicating the city name and weather comment.
Overall, the project provides functionality to fetch weather forecasts, analyze weather data, filter cities based on weather conditions, and visualize the results on a map.

<img width="1131" alt="Screenshot 2023-06-03 at 01 41 29" src="https://github.com/gaurav9189/Weather/assets/28778688/f3e48923-b85a-451f-8c5d-3d0a863756f2">
