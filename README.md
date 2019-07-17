# Bike-Sharing-Prediction-Project
Problem Statement:
After the completion of this project, the Washington D.C city bike sharing program can predict the usage of bikes in different locations and therefore to relocate bikes at low demand area to high demand areas in order to increase the utilization ratio of the bikes.

What will client do or decide based on analysis:
By forecasting bike rental demand of bike sharing program in Washington D.C based on historical usage patterns in relation with weather, time and other factors. People rent a bike from one location and return it to a different or same location on need basis through membership or on demand basis. The city will relocate bicycles based on predictions(i.e. increase or decrease the number of bikes in locations based on weather conditions and time of the day) to meet the demand and maximize the utilization ratio of the bikes, and therefore generate less pollute in the city.

Data Sets:
The data sets are available from this link in .csv format, the data is available from year 2010 to 2019, the data is relatively clean and easy to use. It has the columns of :
duration
start date
end date
start station number
start station location
end station number
end station location
Bike number
Member type

Approach:
The main strategy is to unveil the trend in number of trips started in locations during different time of the day at different dates of the year, the trend in number of trips ends in locations during different time of the day at different dates of the year. From there, by determining the utilization ratio at locations during different time of the day at different dates of the year. Finally, by unveil the trend of trip started in different years in different months.
At different locations, 
utilization ratio is low: (end/ total bike rack) > (start/total bike rack):
need of relocate bikes to high utilization ratio locations or add more bike racks based on the trend;

utilization ratio is high: (start/ total bike rack) > (end/total bike rack):
add more bikes with bike racks based on the trend

Deliverables:
By using python with its packages to combine data in different .csv files and generate data visualization. The code, results, report will be posted on GitHub account.
