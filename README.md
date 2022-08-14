# python-api-challenge
This is my solution to homework #6 for data bootcamp

## Note
In the Outputs folder I have sorted each plot and image into 4 different folders. The scatter plots can be found in the Weather Data Scatter Plotts folder, the Norther and Southern Hemisphere Linear Regression can be found in their own folder by hemisphere, and the images of the heat maps can be found in Map Images. The anyalsis can be found at the end of this README.

## Description
In this challenge I will be taking a list of random cities, finding their weather, and the creating a heatmap of humidity and vacation locations.

To start of I will create list of at least 500 random cities. From there, using the Open Weather Map API, I will create a for loop that will run through all the cities and collect the Latitude, Longitude, Max Temp (F), Humidity, Cloudiness and Wind Speed (mph) information. I will then create a series of plots to see if there are any notible trends between the weather and the latitude of a city.

The next piece is to use this information to find some ideal vacation spots. Using the weather information from before, I will first create a humidity heatmap to have a visual of the most humid places on my list. From their I will find the perfect vacation spots based on my favorite weather, max temp between 65 and 79 F, cloudiness at no more than 30%, humidtiy between 55 and 65%, and wind speeds no more than 9 mph. I will then find the closest hotels to these locations and add markers for each hotel to the heat map

## Analysis on Weather Data
Looking at the City Latitude Vs. Max Temperature scatter plots, we can see that from -50 to 20 degrees latitude the max temp goes up and then from 20 to 80 degrees latitude the max temp goes back down. This can be seen in the curved shaped in the scatter plot with all the data. The Southern Hemisphere linear regression helps supports this claim with a fairly strong r-squared value of 0.6. The Northen Hemisphere linear regression is ok, r-squared of 0.5, but it does of some the curve to it, skewing the linear regression. 

While there is no real relationship between a cities latitude and the wind speed, I did find something intresting in the linear regressions in the Northern and Southern hemisphere. The Southern Hemisphere data is more spread out compared to the Northern Hemisphere. This can be see by the data points, in the Northern Hemisphere most of the data points are within 0 to 15 mph while the Southern Hemisphere is fairly spread out, and with the linear regression lines, the Nothern Hemisphere's line is very flat while the Southern Hemisphere's line is more steep.

Again, whtile there is not relationship between a city's latitude and the humidity, I did find it interesting that a lot of the data points seemed to be 60 or higher. When looking at each Hemisphere's linear regressions the same can be said. For both the Northern and South, most of the data is 60 or above. It makes me wonder if this is becasue of the time of the year, where a lot of my cities close to the equator?