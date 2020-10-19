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

#### Temperature (F) vs. Latitude ####
![ntemp](https://github.com/cveras33/python-api-challenge/blob/main/Images/northern_max_temp_linregress.png)

#### Humidity (%) vs. Latitude ####
![nhumidity](https://github.com/cveras33/python-api-challenge/blob/main/Images/northern_humidity_linregress.png)

#### Cloudiness (%) vs. Latitude ####
![ncloudiness](https://github.com/cveras33/python-api-challenge/blob/main/Images/northern_clousiness_linregress.png)

#### Wind Speed (mph) vs. Latitude ####
![nwindspeed](https://github.com/cveras33/python-api-challenge/blob/main/Images/northern_wind_linregress.png)


### Southern Hemisphere Analysis ### 

#### Temperature (F) vs. Latitude ####
![stemp](https://github.com/cveras33/python-api-challenge/blob/main/Images/southern_max_temp_linregress.png)

#### Humidity (%) vs. Latitude ####
![shumidity](https://github.com/cveras33/python-api-challenge/blob/main/Images/southern_humidity_linregress.png)

#### Cloudiness (%) vs. Latitude ####
![scloudiness](https://github.com/cveras33/python-api-challenge/blob/main/Images/southern_cloudiness_linregress.png)

#### Wind Speed (mph) vs. Latitude ####
![swindspeed](https://github.com/cveras33/python-api-challenge/blob/main/Images/southern_wind_linregress.png)


## Part II: VacationPy ##

#### Heat Map #### 
![headmap](https://github.com/cveras33/python-api-challenge/blob/main/Images/heat_map.png)

#### Hotel Pins #### 
![hotels](https://github.com/cveras33/python-api-challenge/blob/main/Images/hotel_heat_map.png)

### Status ### 
Project is *in progress*. 
