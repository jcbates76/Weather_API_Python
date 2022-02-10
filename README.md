# python-api_challenge
This project contains two parts.  WeatherPy and VacationPy.

## WeatherPy
WeatherPy pulls a list of random latitude and longitude coordinates and matches them to the closest city.  
Pulling from the OpenWeatherMap API, the weather conditions for those cities are pulled and the data analyzed.  
The following charts are created and analyzed to determine relationships:
* Temperature vs Latitude
* Humidity vs Latitude
* Cloudiness vs Latitude
* Wind Speed vs Latitude

All data is analyzed, then the data is split to Northern and Southern Hemispheres and analyzed again utilizing regression analysis.

## VacationPy
Utilizing the dataset from WeatherPy, a heatmap is generated with all cities being identified and humidity being the weight of the heatmap on Google Maps.   
Then, a filter is utilized to select the "ideal" conditions for temperature, humidity, cloudiness and wind speed, to narrow down the list of cities to a select few (under 10 cities) which would be candidates for a vacation just on weather conditions alone.  
The Google Map Heatmap is flagged for those ideal spots and the closest hotel identified in those markers.  
