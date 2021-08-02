# World_Weather_Analysis
An analysis to collect and analyze weather data across cities worldwide.

# Overview

## Purpose
PlanMyTrip will use the data to recommend ideal hotels based on clients' weather preferences.

## Software
Python
Request Version 2.25.1

## Method
Create a Pandas DataFrame with 500 or more of the world's unique cities and their weather data in real time. This process will entail collecting, analyzing, and visualizing the data.
Your analysis of the data will be split into three main parts, or stages.

### Stage 1: Collect the Data
-Use the NumPy module to generate more than 1,500 random latitudes and longitudes.
-Use the citipy module to list the nearest city to the latitudes and longitudes.
-Use the OpenWeatherMap API to request the current weather data from each unique city in your list.
-Parse the JSON data from the API request.
-Collect the following data from the JSON file and add it to a DataFrame:
*City, country, and date
*Latitude and longitude
*Maximum temperature
*Humidity
*Cloudiness
*Wind speed

### Stage 2: Exploratory Analysis with Visualization
-Create scatter plots of the weather data for the following comparisons:
*Latitude versus temperature
*Latitude versus humidity
*Latitude versus cloudiness
*Latitude versus wind speed

-Determine the correlations for the following weather data:
*Latitude and temperature
*Latitude and humidity
*Latitude and cloudiness
*Latitude and wind speed

-Create a series of heatmaps using the Google Maps and Places API that showcases the following:
*Latitude and temperature
*Latitude and humidity
*Latitude and cloudiness
*Latitude and wind speed

### Stage 3: Visualize Travel Data
Create a heatmap with pop-up markers that can display information on specific cities based on a customer's travel preferences. Complete these steps:

-Filter the Pandas DataFrame based on user inputs for a minimum and maximum temperature.
-Create a heatmap for the new DataFrame.
-Find a hotel from the cities' coordinates using Google's Maps and Places API, and Search Nearby feature.
-Store the name of the first hotel in the DataFrame.
-Add pop-up markers to the heatmap that display information about the city, current maximum temperature, and a hotel in the city.


# Results

# Summary


# Analysis Changes
Beta testers recommended a few changes to take the new app to the next level by adding the weather description to the weather data already retrieved and have beta testers use input statements to filter the data for their weather preferences, which will be used to identify potential travel destinations and nearby hotels. From the list of potential travel destinations, the beta tester will choose four cities to create a travel itinerary. Finally, using the Google Maps Directions API, a travel route will be created between the four cities as well as a marker layer map.

## Deliverable 1: Retrieve Weather Data
Generate a set of 2,000 random latitudes and longitudes, retrieve the nearest city, and perform an API call with the OpenWeatherMap. In addition to the city weather data you gathered in this module, use your API skills to retrieve the current weather description for each city. Then, create a new DataFrame containing the updated weather data.

## Deliverable 2: Create a Customer Travel Destinations Map
Use input statements to retrieve customer weather preferences, then use those preferences to identify potential travel destinations and nearby hotels. Then, show those destinations on a marker layer map with pop-up markers.

## Deliverable 3: Create a Travel Itinerary Map
Use the Google Directions API to create a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations. Then, create a marker layer map with a pop-up marker for each city on the itinerary.
