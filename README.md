# Bike renting case study

## Table of Contents

* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## Introduction

Business Problem: A bike renting business Boombike, severely impacted by covid is struggling to survive. They are looking  to make strategic decisions and come up with a business plan after lockdown.
 Based on the meteorological data collected over the last two years , they want to undestand:
 
  Which variables are significant in predicting the demand for shared bikes.
  How well those variables describe the bike demands

The aim of this work is to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.


# Dataset characteristics

day.csv have the following fields:
	
	- instant: record index
	- dteday : date
	- season : season (1:spring, 2:summer, 3:fall, 4:winter)
	- yr : year (0: 2018, 1:2019)
	- mnth : month ( 1 to 12)
	- holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
	- weekday : day of the week
	- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
	+ weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
	- temp : temperature in Celsius
	- atemp: feeling temperature in Celsius
	- hum: humidity
	- windspeed: wind speed
	- casual: count of casual users
	- registered: count of registered users
	- cnt: count of total rental bikes including both casual and registered
	
## Conclusions

The top five factors contributing to demand of rented bikes are as below:
year of renting (rate of change ~25% )
feeling temprature (rate of change ~ 46%)
humidity (rate of change ~-27%)
windspeed (rate of change ~ -22%)
Spring season (rate of change ~ -17%)
The model strongly suggests that business can expect growth in coming years. The temprature rise causes a positive impact on the demand for bikes. Overall, the humidity, windspeed Spring season is when the demand for bike dips

Please note the model is able to describe roughly .757 variance of bike demand.

## Technologies Used

seaborn 0.11.1
jupyter 1.0.0
numpy 1.20.1
anaconda 2021.05
python 3.8.8 
matplotlib 3.3.4
Microsoft excel


## Contact

Created by [@NavsGo] - feel free to contact me!
