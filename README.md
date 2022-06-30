# World_Weather_Analysis
An weather analysis to collect and analyze weather data across cities worldwide.

# Overview
Using APIs to Visualize Weather Data

## Purpose
PlanMyTrip used the data to recommend ideal hotels based on clients' weather preferences.

### Resources
Data Source: WeatherPy_Database.csv (generated from OpenWeatherMap API Request)
Software: Conda 4.10.3, Python 3.7.6, Jupyter Notebook 6.3.0, Pandas, Matplotlib, and Request Version 2.25.1

## Method Used
A Pandas DataFrame was created with 500 or more of the world's unique cities and their weather data in real time. This process entailed collecting, analyzing, and visualizing the data.
The analysis of the data was split into three main parts, or stages.

### Stage 1: Collection of Data
-- NumPy module was used to generate more than 2,000 random latitudes and longitudes.
-- Citipy module was used to list the nearest city to the latitudes and longitudes.
-- OpenWeatherMap API was used to request the current weather data from each unique city in the list.
-- JSON data was parsed from the API request.
-- The following data was collected from the JSON file and added to a DataFrame:
* City, country, and date
* Latitude and longitude
* Maximum temperature
* Humidity
* Cloudiness
* Wind speed

### Stage 2: Exploratory Analysis with Visualization
-- Scatter plots of the weather data for the following comparisons were created:
* Latitude versus temperature
* Latitude versus humidity
* Latitude versus cloudiness
* Latitude versus wind speed

-- Correlations for the following weather data were determined:
* Latitude and temperature
* Latitude and humidity
* Latitude and cloudiness
* Latitude and wind speed

-- A series of heatmaps using the Google Maps and Places API that showcases the following was created:
* Latitude and temperature
* Latitude and humidity
* Latitude and cloudiness
* Latitude and wind speed

### Stage 3: Visualize Travel Data
-- A heatmap with pop-up markers that displayed information on specific cities based on a customer's travel preferences was created. The following steps were completed:

* The Pandas DataFrame was filtered based on user inputs for a minimum and maximum temperature.
* A heatmap was created for the new DataFrame.
* A hotel was found from the cities' coordinates using Google's Maps and Places API, and Search Nearby feature.
* The name of the first hotel was stored in the DataFrame.
* Pop-up markers were added to the heatmap that displayed information about the city, current maximum temperature, and a hotel in the city.

# Analysis Changes and Results
Beta testers recommended a few changes to take the new app to the next level by adding the weather description to the weather data already retrieved and have beta testers use input statements to filter the data for their weather preferences, which will be used to identify potential travel destinations and nearby hotels. From the list of potential travel destinations, the beta tester will choose four cities to create a travel itinerary. Finally, using the Google Maps Directions API, a travel route will be created between the four cities as well as a marker layer map.

## Deliverable 1: Retrieve Weather Data Retrieved
Generate a set of 2,000 random latitudes and longitudes, retrieve the nearest city, and perform an API call with the OpenWeatherMap. In addition to the city weather data you gathered in this module, use your API skills to retrieve the current weather description for each city. Then, create a new DataFrame containing the updated weather data.

### Deliverable 1 Results: Collect the Data
-- Out of the 2,000 random latitudes and longitudes that were generated, 757 nearest cities were listed with 688 of those cities generating data and stored in the Weather_Database. 
![city_data_dataframe.png](https://github.com/KimberlyCrawford/World_Weather_Analysis/blob/main/RESOURCES/city_data_dataframe.png)

## Deliverable 2: Create a Customer Travel Destinations Map
Use input statements to retrieve customer weather preferences, then use those preferences to identify potential travel destinations and nearby hotels. Then, show those destinations on a marker layer map with pop-up markers.

### Deliverable 2 Results: Exploratory Analysis with Visualization
-- Based on customer weather preferences of 72 minimum temp and 80 maximum temp, below is a map of potential travel destinations and nearby hotels. 
![WeatherPy_vacation_map.png](https://github.com/KimberlyCrawford/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)

## Deliverable 3: Create a Travel Itinerary Map
Use the Google Directions API to create a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations. Then, create a marker layer map with a pop-up marker for each city on the itinerary.

### Deliverable 3 Results: Visualize Travel Data
-- Below is the travel itinerary map.
![WeatherPy_travel_map.png](https://github.com/KimberlyCrawford/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)

#### Module 6, Data Analysis & Visualization Certificate Program, UT Austin McCombs School of Business, 2021.
