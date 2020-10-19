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

To briefly discuss latitude, which is the measure the x-axis focuses on in the above, and next three scatter plots; it is a city's north-south position, where latitude at the equator is measured as 0&deg; and increases towards 90&deg; as a city gets closer to the north pole and decreases towards -90° as a city gets closer to the south pole.

#### Temperature (F) vs. Latitude ####
![temp](https://github.com/cveras33/python-api-challenge/blob/main/Images/lat_vs_temp.png)

The above scatter plot vizualizes how a world city's latitute is related to the city's temperature. As mentioned above, the equator sits at 0° latitude, and based off what we can see in this plot, as a city's latitude gets closer to 0&deg;, it's maximum temperature is greater. Whereas city's whose latitude is further from 0&deg;, have lower maximum temperatures. Therefore, it can be concluded based on the data visualization, that city's that are closer to the equator are warmer than cities that are further away.

#### Humidity (%) vs. Latitude ####
![humidity](https://github.com/cveras33/python-api-challenge/blob/main/Images/lat_vs_humidity.png)

This next scatter plot shows the relationship between a world city's latitude and the humidity in that city. As shown in the scatter plot, there is really no clear relationship between latitude and humidity, but there is a larger cluster of data points in the top righthand corner of the plot, so maybe there is something to say about cities closer to the north pole with higher temperatures, but nothing can be determined from this plot.

#### Cloudiness (%) vs. Latitude ####
![cloudiness](https://github.com/cveras33/python-api-challenge/blob/main/Images/lat_vs_cloudiness.png)

Similarly to the humidity scatter plot, this plot, which looks at the relationship between city latitude and cloudiness does not indicate any strong relationship between the two. Again, there are more densely clustered data points along the bottom and top of the plot, where 0% cloudiness and 100% cloudiness data points sit, but nothing definitive can be said about this relationship based on this plot.

#### Wind Speed (mph) vs. Latitude ####
![windspeed](https://github.com/cveras33/python-api-challenge/blob/main/Images/lat_vs_wind_speed.png)

This last scatter plot looks at the relationship between city latitude and wind speed. The data points are most densely populated all along the bottom of the graph, with a pretty even spread of datapoints having higher wind speeds. Again, it would be pretty difficult to say anything about the relationship between latitude and wind speed based solely off the scatter plot shown.

### Northern Hemisphere Analysis ### 

#### Temperature (F) vs. Latitude ####
![ntemp](https://github.com/cveras33/python-api-challenge/blob/main/Images/northern_max_temp_linregress.png)

The linear regression plot above shows the relationship between latitude in the northern hemisphere and the max temperature. Temperature and latitude have a negative correlation in the northern hemisphere, which can be seen in the plot, since a greater latitude is associated with lower temperatures and vice versa. It can also be determined by the r-value that the two variables are closely related, based on how close the value is to -1.

#### Humidity (%) vs. Latitude ####
![nhumidity](https://github.com/cveras33/python-api-challenge/blob/main/Images/northern_humidity_linregress.png)

The linear regression plot above shows the relationship between latitude in the nothern hemisphere and humidity. Temperature and latitude have a positive correlation in the northern hemisphere, which can be seen in the plot, since a greater latitude is associated with greater humidity. The two variables here are not strongly correlated, which, again, we can determine by the r-value, which in this class is much closer to 0 than it is to 1.

#### Cloudiness (%) vs. Latitude ####
![ncloudiness](https://github.com/cveras33/python-api-challenge/blob/main/Images/northern_clousiness_linregress.png)

The linear regression plot above shows the relationship between latitude in the northern hemisphere and cloud coverage. Cloud coverage and latitude have a positive correlation in the northern hemisphere. Again, looking at the data points alone, it is difficult to come to that conclusion, but the linear regression line helps give a bit more indication as that. We can also tell there is a lack of correlation between the two variables here because the r-value is fairly close to 0.

#### Wind Speed (mph) vs. Latitude ####
![nwindspeed](https://github.com/cveras33/python-api-challenge/blob/main/Images/northern_wind_linregress.png)

The linear regression plot above shows the relationship between latitude in the northern hemisphere and wind speed measured in MPH. Wind speed and latitude have a positive correlation in the northern hemisphere. Still, there is no great correlation between the two variables in this plot, as shown by the r-value being so close to 0.

### Southern Hemisphere Analysis ### 

#### Temperature (F) vs. Latitude ####
![stemp](https://github.com/cveras33/python-api-challenge/blob/main/Images/southern_max_temp_linregress.png)

The linear regression plot above shows the relationship between latitude in the southern hemisphere and the max temperature. Temperature and latitude have a positive correlation in the southern hemisphere, which can be seen in the plot, since a greater latitude is associated with greater temperatures. Although, the correlation between the two variables is not as great as the correlation between latitude and temperature in the northern hemisphere.

#### Humidity (%) vs. Latitude ####
![shumidity](https://github.com/cveras33/python-api-challenge/blob/main/Images/southern_humidity_linregress.png)

The linear regression plot above shows the relationship between latitude in the souther hemisphere and humidity. Temperature and latitude again, have a positive correlation in the northern hemisphere, which is represented by the positively sloped linear regression line in the plot. But looking at the data points alone, it would be somewhat difficult to determine that. The two variables here are almost not correlated at all based on the very very low r-value.

#### Cloudiness (%) vs. Latitude ####
![scloudiness](https://github.com/cveras33/python-api-challenge/blob/main/Images/southern_cloudiness_linregress.png)

The linear regression plot above shows the relationship between latitude in the southern hemisphere and cloud coverage. Cloud coverage and latitude have a positive correlation in the southern hemisphere as well. The date points alone here also do not give a great indication of that.

#### Wind Speed (mph) vs. Latitude ####
![swindspeed](https://github.com/cveras33/python-api-challenge/blob/main/Images/southern_wind_linregress.png)

The linear regression plot above shows the relationship between latitude in the southern hemisphere and wind speed measured in MPH. Wind speed and latitude have a negative correlation in the southern hemisphere, differing from the relationship between wind speed and latitude in the northern hemisphere. Similarly to the northern hemisphere, there is no great correlation between wind speed and latitude in the southern hemisphere, as shown by the r-value being so close to 0.

## Part II: VacationPy ##

#### Heat Map #### 
![headmap](https://github.com/cveras33/python-api-challenge/blob/main/Images/heat_map.png)

#### Hotel Pins #### 
![hotels](https://github.com/cveras33/python-api-challenge/blob/main/Images/hotel_heat_map.png)

### Status ### 
Project is *in progress*. 
