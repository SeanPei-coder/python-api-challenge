# python-api-challenge
## Part I - WeatherPy

In this part, I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I utilized a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.

I created a series of scatter plots to showcase the following relationships:

Temperature (F) vs. Latitude

![alt text](https://github.com/SeanPei-coder/python-api-challenge/blob/main/WeatherPy/Output/City%20Latitude%20vs.%20Max%20Temperature.png)


Humidity (%) vs. Latitude

![alt text](https://github.com/SeanPei-coder/python-api-challenge/blob/main/WeatherPy/Output/City%20Latitude%20vs.%20Humidity.png)


Cloudiness (%) vs. Latitude

![alt text](https://github.com/SeanPei-coder/python-api-challenge/blob/main/WeatherPy/Output/City%20Latitude%20vs.%20Cloudiness.png)


Wind Speed (mph) vs. Latitude

![alt text](https://github.com/SeanPei-coder/python-api-challenge/blob/main/WeatherPy/Output/City%20Latitude%20vs.%20Wind%20Speed.png)


Next, I ran linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

Northern Hemisphere - Temperature (F) vs. Latitude

![alt text](https://github.com/SeanPei-coder/python-api-challenge/blob/main/WeatherPy/Output/latitude%20and%20max%20temperature%20for%20northern%20hemisphere.png)

The r-value is: -0.8441204881300122

There is a strong negative relationship between latitude and max temperature for northern hemisphere.



Southern Hemisphere - Temperature (F) vs. Latitude

![alt text](https://github.com/SeanPei-coder/python-api-challenge/blob/main/WeatherPy/Output/latitude%20and%20max%20temperature%20for%20southern%20hemisphere.png)

The r-value is: 0.7328686011085312

There is a strong positive relationship between latitude and max temperature for southern hemisphere.



Northern Hemisphere - Humidity (%) vs. Latitude

![alt text](https://github.com/SeanPei-coder/python-api-challenge/blob/main/WeatherPy/Output/latitude%20and%20humidity%20for%20northern%20hemisphere.png)

The r-value is: 0.07297858985545783

There is a weak positive relationship between latitude and humidity for northern hemisphere.



Southern Hemisphere - Humidity (%) vs. Latitude

![alt text](https://github.com/SeanPei-coder/python-api-challenge/blob/main/WeatherPy/Output/latitude%20and%20humidity%20for%20southern%20hemisphere.png)

The r-value is: 0.14169467867351068

There is a weak positive relationship between latitude and humidity for southern hemisphere.



Northern Hemisphere - Cloudiness (%) vs. Latitude

![alt text](https://github.com/SeanPei-coder/python-api-challenge/blob/main/WeatherPy/Output/latitude%20and%20cloudiness%20for%20northern%20hemisphere.png)

The r-value is: 0.06927616638120615

There is a weak positive relationship between latitude and cloudiness for northern hemisphere.



Southern Hemisphere - Cloudiness (%) vs. Latitude

![alt text](https://github.com/SeanPei-coder/python-api-challenge/blob/main/WeatherPy/Output/latitude%20and%20cloudiness%20for%20southern%20hemisphere.png)

The r-value is: 0.024052339231411576

There is a weak positive relationship between latitude and cloudiness for southern hemisphere.



Northern Hemisphere - Wind Speed (mph) vs. Latitude

![alt text](https://github.com/SeanPei-coder/python-api-challenge/blob/main/WeatherPy/Output/latitude%20and%20wind%20speed%20for%20northern%20hemisphere.png)

The r-value is: 0.024052339231411576

There is a weak positive relationship between latitude and cloudiness for southern hemisphere.


Southern Hemisphere - Wind Speed (mph) vs. Latitude

![alt text](https://github.com/SeanPei-coder/python-api-challenge/blob/main/WeatherPy/Output/latitude%20and%20wind%20speed%20for%20southern%20hemisphere.png)

The r-value is: -0.21396157407190491

There is a weak negative relationship between latitude and wind speed for southern hemisphere.


## Part II - VacationPy
I created a heat map that displays the humidity for every city from the part I of the work.
![alt text](https://github.com/SeanPei-coder/python-api-challenge/blob/main/VacationPy/Output/output1.png)

Then, I narrow down the DataFrame:

200 < Max Temp <300 

Wind Speed < 7 MPH

Cloudiness < 70%
                            
I Use Google Places API to find the first hotel for each city located within 5000 meters of the coordinates, and plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.

![alt text](https://github.com/SeanPei-coder/python-api-challenge/blob/main/VacationPy/Output/output2.png)
