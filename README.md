# python-api_challenge
This project contains two parts.  WeatherPy and VacationPy.

## WeatherPy
WeatherPy pulls a list of random latitude and longitude coordinates and matches them to the closest city.  
Pulling from the OpenWeatherMap API, the weather conditions for those cities are pulled and the data analyzed.  
The following charts are created and analyzed to determine relationships:
* Temperature vs Latitude
![Temp_Lat](https://user-images.githubusercontent.com/94392882/188523550-de8e61e0-d84a-490c-b5dd-da3e6898c4af.png)
* Humidity vs Latitude
![Humidity_Lat](https://user-images.githubusercontent.com/94392882/188523565-1936fedd-a4aa-4367-8381-f7d56107e904.png)
* Cloudiness vs Latitude
![Clouds_Lat](https://user-images.githubusercontent.com/94392882/188523574-979ca442-b9a1-4ce0-8c11-54caa135f047.png)
* Wind Speed vs Latitude
![Wind_Lat](https://user-images.githubusercontent.com/94392882/188523583-0f660d94-e295-4a98-bc85-9a150d67095e.png)
All data is analyzed, then the data is split to Northern and Southern Hemispheres and analyzed again utilizing regression analysis.

## VacationPy
Utilizing the dataset from WeatherPy, a heatmap is generated with all cities being identified and humidity being the weight of the heatmap on Google Maps.   
Then, a filter is utilized to select the "ideal" conditions for temperature, humidity, cloudiness and wind speed, to narrow down the list of cities to a select few (under 10 cities) which would be candidates for a vacation just on weather conditions alone.  
The Google Map Heatmap is flagged for those ideal spots and the closest hotel identified in those markers.  
![Heatmap with Hotels](https://user-images.githubusercontent.com/94392882/188523607-6842ce6b-7f3d-4631-b852-847ff2c560c9.png)
