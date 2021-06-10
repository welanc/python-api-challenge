# Python API Challenge

## Task

### WeatherPy Directory

Two Jupyter Notebooks used to explore and visualise the weather of 500+ cities across the world of varying distance from the equator.

**WeatherPy.ipynb**
API call to Open WeatherMap Org. (requires API key in api_keys.py) using a try and except function to continue running through key errors, search for nearest city based on randomly generated geographic coordinates and relevant weather data for each location. API called data is transformed into a Pandas Dataframe and numerous scatter plots produced and linear regression analyses performed to analyse the dataset. 

Scatter plots include, with a brief sentence analysing the data:
* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

Scatter plots with linear regression and brief sentence analysing the data: 
* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude
 
Export dataset for use in VacationPy.ipynb


**VacationPy.ipynb**

Plot a heatmap to visualise the humidity of every city from the WeatherPy dataset using Google Places API.

Based on the API data retrieved from WeatherPy, VacationPy is used to determine ideal vacation locations that meets all three of the following weather criteria: 

* A max temperature lower than 80 degrees (Fahrenheit) but higher than 70.
* Wind speed less than 10 mph.
* Zero cloudiness.

Once the locations are determined, using Google Places API, plot a marker of the first hotel within 5,000 metres of each ideal city's coordinates. A pin with info box contains: Hotel Name, City and Country. 


### Output Data Directory

Output files from WeatherPy.ipynb:
* CSV:
  * cities.csv - contains weather data for randomly generated selection of cities.
* PNG:
  * Fig1.png - Temperature (F) vs. Latitude
  * Fig2.png - Humidity (%) vs. Latitude
  * Fig3.png - Cloudiness (%) vs. Latitude
  * Fig4.png - Wind Speed (mph) vs. Latitude
  * Fig5.png - Northern Hemisphere - Temperature (F) vs. Latitude
  * Fig6.png - Southern Hemisphere - Temperature (F) vs. Latitude
  * Fig7.png - Northern Hemisphere - Humidity (%) vs. Latitude
  * Fig8.png - Southern Hemisphere - Humidity (%) vs. Latitude
  * Fig9.png - Northern Hemisphere - Cloudiness (%) vs. Latitude
  * Fig10.png - Southern Hemisphere - Cloudiness (%) vs. Latitude
  * Fig11.png - Northern Hemisphere - Wind Speed (mph) vs. Latitude
  * Fig12.png - Southern Hemisphere - Wind Speed (mph) vs. Latitude

Output files from WeatherPy.ipynb:
* PNG:
  * map_heatmap.png
  * map_markers.png


--- 

## Technologies

* Jupyter Notebook
* OpenWeatherMap.org API
* Google Places API

Python Libraries:
* Pandas
* Numpy
* MatPlotLib
* scipy
  * stats
* json
* citipy
* random
* requests
* gmaps
* os
  

