# Python API Challenge - What's the weather like? 

## Background ##

Using Python requests, APIs and JSON traversals, the following weather analysis answers the questsion __"What's the weather like as we approach the equator?"__. Using data from the [Open Weather Map API](https://openweathermap.org/api), the previously stated question is answered by getting data about 500+ world cities with varying distance from the equator, which is located at 0&deg; latitude, creating an imaginary line between the northern and southern hemispheres of the globe. Going one step further, the data about world cities retieved from the Open Weather API, along with [Google Places API](https://developers.google.com/places/web-service/overview) and jupyter-gmaps is used to plan future vacations in world cities only with ideal weather conditions. 

## Table of Contents ## 
* [Part I: WeatherPy](#part-i-weatherpy)
  * [Northern Hemisphere Analysis](#northern-hemisphere-analysis)
  * [Southern Hemisphere Analysis](#southern-hemisphere-analysis)
* [Part II: VacationPy](#part-ii-vacationpy)


## Part I: WeatherPy ## 
After performing a series of API calls to the Open Weather Map API, world city data is stored in the [weather_check.csv](https://github.com/cveras33/python-api-challenge/blob/main/Output/weather_check.csv) file, which can be accessed via the link or found in the Output folder in this repository. The data was then used to create the following scatter plots to show case the following relationships: 

#### Temperature (F) vs. Latitude ####
![temp](https://github.com/cveras33/python-api-challenge/blob/main/Images/lat_vs_temp.png)

#### Humidity (%) vs. Latitude ####
![humidity](https://github.com/cveras33/python-api-challenge/blob/main/Images/lat_vs_humidity.png)

#### Cloudiness (%) vs. Latitude ####
![cloudiness](https://github.com/cveras33/python-api-challenge/blob/main/Images/lat_vs_cloudiness.png)

#### Wind Speed (mph) vs. Latitude ####
![windspeed](https://github.com/cveras33/python-api-challenge/blob/main/Images/lat_vs_wind_speed.png)


### Northern Hemisphere Analysis ### 

### Southern Hemisphere Analysis ### 

## Part II: VacationPy ##

### Status ### 
Project is *in progress*. 
