# python_api_challenge
This module analyzes weather trends over 500 cities
Instructions for this module provided by Columbia University Data Analytics Bootcamp.

Instructions
This activity is broken down into two deliverables, WeatherPy and VacationPy.

Part 1: WeatherPy
In this deliverable, you'll create a Python script to visualize the weather of over 500 cities of varying distances from the equator. You'll use the citipy Python libraryLinks and the OpenWeatherMap APILinks.
Generate random geographic coordinates and the nearest city to each latitude and longitude combination.

Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
Create a series of scatter plots to showcase the following relationships:
  Latitude vs. Temperature
  Latitude vs. Humidity
  Latitude vs. Cloudiness
  Latitude vs. Wind Speed

Requirement 2: Compute Linear Regression for Each Relationship
Compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). 
Next, create a series of scatter plots. Be sure to include the linear regression line, the model's formula, and the r values.
You should create the following plots:
  Northern Hemisphere: Temperature vs. Latitude
  Southern Hemisphere: Temperature vs. Latitude
  Northern Hemisphere: Humidity vs. Latitude  
  Southern Hemisphere: Humidity vs. Latitude
  Northern Hemisphere: Cloudiness vs. Latitude
  Southern Hemisphere: Cloudiness vs. Latitude
  Northern Hemisphere: Wind Speed vs. Latitude
  Southern Hemisphere: Wind Speed vs. Latitude

Part 2: VacationPy
Use the geoViews Python library and the Geoapify API.

Create a map that displays a point for every city in the city_data_df DataFrame. The size of the point should be the humidity in each city.

Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:
  A max temperature lower than 27 degrees but higher than 21
  Wind speed less than 4.5 m/s
  Zero cloudiness

Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.
For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.
Add the hotel name and the country as additional information in the hover message for each city on the map.

To be thorough, a map was created with every city from the hotel_df regardless of whether a hotel was found within each of those cities. And another map was created only including those ideal cities from the hotel_df that had a hotel within 10,000 meters.

Resources:
https://bootcampspot.instructure.com/courses/4737/assignments/68524?module_item_id=1161640
https://openweathermap.org/api
https://www.geoapify.com/
https://openweathermap.org/current#example_JSON
https://stackoverflow.com/questions/50706901/matplotlib-border-around-scatter-plot-points
https://stackoverflow.com/questions/59678780/show-extra-columns-when-hovering-in-a-scatter-plot-with-hvplot#:~:text=1%20Answer&text=You%20can%20use%20keyword%20hover_cols%20to%20add%20additional%20columns%20to%20your%20hover.&text=Additional%20columns%20to%20add%20to,indexes%20if%20use_index%20is%20True).&text=Amazing%2C%20exactly%20what%20I%20was%20looking%20for.
https://apidocs.geoapify.com/docs/places/#categories
