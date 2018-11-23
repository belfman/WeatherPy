# WeatherPy 
<a href = "https://belfman.github.io/index.html"> Link to WeatherPy Page</a> 


### Task
Use data analytics to answer and visualize this question: __is it hotter at the equator?__
***
### Process
First, I used the Random module in Python to uniformly select Latitudes between -90.000 to 90.000, and Longitudes
from -180.000 to 180.000. I generated 2000 unique coordinate pairs. 
Second, I used the Citipy module to find the nearest city to each coordinate pair, and eliminated any duplicates.
This left me with an unbiased sample of 637 cities.
Third, I queried the OpenWeatherMap website to get relevant data for each city such as: temperature, % humidity, % cloudiness,
wind speed.
Finally, I used pandas and matplotlib to create a DataFrame and visualize the results.

![](images/Latitude_Longitude.png "it's a small (hello)world")

# Analysis
There is a clear correlation of latitude to temperature. As the latitudes approach the extreme values, the temperature
decreases, with the highest temperatures found at 35 degrees. With a larger data set, the trend could lean more to 
higher temperatures closer to zero degrees. 
As for % humidity and the other graphs made, there is no correlation to be found based on latitude. There is an even
distribution of humidity, cloudiness and wind speed accross all the latitudes. 

![](images/Latitude_Temperature.png "its hot hot hot!")


![](images/Latitude_Humidity.png "good for plants")


![](images/Latitude_Cloudiness.png "with a chance of meatballs")


![](images/Latitude_Wind.png "Chi-ca-go! you're out!")
