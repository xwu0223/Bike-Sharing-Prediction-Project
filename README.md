# Bike-Sharing-Prediction-Project
Problem Statement:
After the completion of this project, the Washington D.C city bike sharing program can predict the usage of bikes in different locations and therefore to relocate bikes at low demand area to high demand areas in order to increase the utilization ratio of the bikes.

What will client do or decide based on analysis:
By forecasting bike rental demand of bike sharing program in Washington D.C based on historical usage patterns in relation with weather, time and other factors. People rent a bike from one location and return it to a different or same location on need basis through membership or on demand basis. The city will relocate bicycles based on predictions(i.e. increase or decrease the number of bikes in locations based on weather conditions and time of the day) to meet the demand and maximize the utilization ratio of the bikes, and therefore generate less pollute in the city.

Data Sets:
The data sets are available from this link in .csv format, the data is available from year 2011 to 2012, the data is relatively clean and easy to use. It has the columns of :
	- instant: record index
	- dteday : date
	- season : season (1:springer, 2:summer, 3:fall, 4:winter)
	- yr : year (0: 2011, 1:2012)
	- mnth : month ( 1 to 12)
	- hr : hour (0 to 23)
	- holiday : weather day is holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
	- weekday : day of the week
	- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
	+ weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
	- temp : Normalized temperature in Celsius. The values are divided to 41 (max)
	- atemp: Normalized feeling temperature in Celsius. The values are divided to 50 (max)
	- hum: Normalized humidity. The values are divided to 100 (max)
	- windspeed: Normalized wind speed. The values are divided to 67 (max)
	- casual: count of casual users
	- registered: count of registered users
	- cnt: count of total rental bikes including both casual and registered

Approach:
The main strategy is to unveil the trend in number of trips started in locations during different time of the day at different dates of the year, the trend in number of trips ends in locations during different time of the day at different dates of the year. From there, by determining the utilization ratio at locations during different time of the day at different dates of the year. Finally, by unveil the trend of trip started in different years in different months.
At different locations, 
utilization ratio is low: (end/ total bike rack) > (start/total bike rack):
need of relocate bikes to high utilization ratio locations or add more bike racks based on the trend;

utilization ratio is high: (start/ total bike rack) > (end/total bike rack):
add more bikes with bike racks based on the trend

Deliverables:
By using python with its packages to combine data in different .csv files and generate data visualization. The code, results, report will be posted on GitHub account.
