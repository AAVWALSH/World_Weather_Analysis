# World_Weather_Analysis

The purpose was to add additional functionality to the PlanMyTrip app to allow users to input statements to filter the results based on the weather preferences of potential travel destinations.  


### Retrieve Weather Data

The Weather_Database.ipynb generates a set of 2000 random coordinates, used CityPY to find the nearest city, and then performs an API call with OpenWeatherMap to find local weather details for that city. The API call specifically sought the maximum temperature, the percent humidity, percent cloudiness, wind speed, and current weather description. The data was saved to the WeatherPy_Database.csv file. 

### Customer Travel Destinations Map
The Vacation_Search.ipynb allows a customer to enter some parameters of max and min temperatures to find an ideal vacation destinations and nearby hotels. Once the max and min temparatures are provided a Google Maps API call provides hotels within 5000m of each city that mets the requested temperature range. An interactive map is generated with pop-up markers that can be selected to show additional information such as hotel name, city, country, and current weather. 

![WeatherPy_Vacation_map](https://user-images.githubusercontent.com/100727593/163696880-dc8dd523-7454-49af-9cba-9bcd7391b8f1.png)


### Travel Itinerary Map
The Vacation_Itinerary.ipynb uses a Google Directions API call to show a route between four cities chosen fom the customer's possible travel destinations. The example in the attached shows a possible route between 4 cities in southern Mexico. 
![WeatherPy_travel_map](https://user-images.githubusercontent.com/100727593/163696903-24a1b5f8-f145-4eb2-8212-99334a811d9f.png)
