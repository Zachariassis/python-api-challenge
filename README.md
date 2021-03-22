# python-api-challenge

This project uses real-time weather data to predict a vacation destination. This projects has two parts; WeatherPy.ipynb and VacationPy.ipynb. 

The first code file to be run should be WeatherPy.ipynb. 550 cities are randomly selected from a list in [Citypy](https://pypi.org/project/citipy/). Humidity, rainfall, cloudiness, and wind speed are compared between all cities based on their longitude and latitude. This information is saved for the next portion of the project. 

Optical vacation weather parameters are defined in VacationPy. These were used to determine a subset of the cities that would be great places to vacation. Once cities are identified using google maps a hotel is located in that city for the vacation. Happy hunting!

This code uses real-time data, thus results will vary with time of year. 

Max temperature correlated with distance from the equator for both hemispheres. This was expected.

Most of the data found trended towards coastal cities. This was a function of the random number generator used to find random coordinates on the graph, and the fact that the earth is majority water, thus the closest city would be coastal. This may affect certain relationships as oceanic weather may differ from inland. 

There were relatively few cities with low humidity near the equator and most humidities were quite high. Again this is probably biased by the oceananic cities. Also not many cities in deserts near the equator. 

To run this code you will need a working api key from [open weather map](https://openweathermap.org/api). You will place this key in a new file in this folder called api_keys.py under the variable name "weather_api_key"

In addition you will also need a [google maps api key](https://developers.google.com/maps). This key will be in the same api_keys.py file under the variable name "g_key"
