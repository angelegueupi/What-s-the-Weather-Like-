# Python API  - What's the Weather Like?
Background
![equatorsign](https://user-images.githubusercontent.com/106934375/197659244-f04529b3-a599-4957-9f9f-136216b1a0d0.png)

Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. So let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

Now, we know what you may be thinking: "Duh. It gets hotter..."

But, if pressed, how would you prove it?

## Part I - WeatherPy

In this example, you'll be creating a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, you'll be utilizing a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.

Your first objective is to build a series of scatter plots to showcase the following relationships:

Temperature (F) vs. Latitude
Humidity (%) vs. Latitude
Cloudiness (%) vs. Latitude
Wind Speed (mph) vs. Latitude

![image](https://user-images.githubusercontent.com/106934375/197660072-159f2cbe-0929-473a-8d8e-3835ede972c0.png)

After each plot add a sentence or too explaining what the code is and analyzing.

Your next objective is to run linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

Northern Hemisphere - Temperature (F) vs. Latitude
Southern Hemisphere - Temperature (F) vs. Latitude
Northern Hemisphere - Humidity (%) vs. Latitude
Southern Hemisphere - Humidity (%) vs. Latitude
Northern Hemisphere - Cloudiness (%) vs. Latitude
Southern Hemisphere - Cloudiness (%) vs. Latitude
Northern Hemisphere - Wind Speed (mph) vs. Latitude
Southern Hemisphere - Wind Speed (mph) vs. Latitude

After each pair of plots explain what the linear regression is analyzing, any relationships you notice and any other analysis you may have.

Your final notebook must:

Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
Perform a weather check on each of the cities using a series of successive API calls.
Include a print log of each city as it's being processed with the city number and city name.
Save a CSV of all retrieved data and a PNG image for each scatter plot.

## Part II - VacationPy

Now let's use your skills in working with weather data to plan future vacations. Use Jupyter gmaps and the Google Places API for this part of the assignment.

Note: if you having trouble displaying the maps try running jupyter nbextension enable --py gmaps in your environment and retry.

Create a heat map that displays the humidity for every city from the part I of the homework.

![heatmap](https://user-images.githubusercontent.com/106934375/197658749-7ae830ba-268a-4c1b-9dd8-2c2bc7ac54ef.png)


Narrow down the DataFrame to find your ideal weather condition. For example:

A max temperature lower than 80 degrees but higher than 70.

Wind speed less than 10 mph.

Zero cloudiness.

Drop any rows that don't contain all three conditions. You want to be sure the weather is ideal.

Note: Feel free to adjust to your specifications but be sure to limit the number of rows returned by your API requests to a reasonable number.

Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.

Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.
![hotel_map](https://user-images.githubusercontent.com/106934375/197658808-5dee18c5-bf6a-4683-a575-7c317bf9f174.png)
