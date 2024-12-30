# Bike renting case study

## Table of Contents

* [General Info](#general-information)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)
* [Dataset characteristics](#dataset-characteristics)
* [Acknowledgements](#acknowledgements)


## Introduction

**Business Problem**: A bike renting business Boombike, severely impacted by covid is struggling to survive. They are looking  to make strategic decisions and come up with a business plan after lockdown.
 Based on the meteorological data collected over the last two years , they want to undestand: 
  - which variables are significant in predicting the demand for shared bikes.
  - how well those variables describe the bike demands

The aim of this case study is to model the demand for shared bikes with the available independent variables. The model will be a good way for management to understand the demand dynamics of a new market. They can then accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. 
	
## Conclusions

The top five factors contributing to demand of rented bikes are as below:
- feeling temperature (rate of change ~ **+46%**) i.e. a 100C increase in 'feeling temperature' will result approx 46 more bikes demand
- humidity (rate of change ~-**-27%**) i.e. a 100 unit increased in humidity will reduce bike sharing demand by approx 27 bikes.
- year of renting (rate of change **~ +25%** ) i.e. each year we are expecting 25% increase in bike sharing demand
- windspeed (rate of change ~ **-22%)** i.e. a 100 unit change in windspeed will result approx 22 more bikes demand.
- Spring season (rate of change ~ **-17%**)  i.e. if the demand was 100 before Spring, the demand will reduce to 83 in spring.
  The model strongly suggests that business can expect growth in coming years. The temperature rise causes a positive impact on the demand for bikes. An increase in humidity, windspeed & Spring season causes a dip in demand for shared bikes

Please note the model is able to describe ~ **.757** variance of bike demand.

## Technologies Used

- seaborn 0.11.1
- jupyter 1.0.0
- numpy 1.20.1
- anaconda 2021.05
- python 3.8.8 
- matplotlib 3.3.4
- Microsoft excel

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

## Contact

Created by [@NavsGo](@navsgo) - feel free to contact me!
