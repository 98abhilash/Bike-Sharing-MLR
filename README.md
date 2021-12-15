# Assignment - Multiple Linear Regression (Bike Sharing Data)

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
<!--  -->
<!-- You can include any other section that is pertinent to your problem -->

## General Information
### Problem Statement

A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.<br>
A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.<br> 
In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.<br>
They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. <br>The company wants to know:

1. Which variables are significant in predicting the demand for shared bikes.
2. How well those variables describe the bike demands<br>

Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.


### Business Goal

You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 

### Data Dictionary 

#### Dataset characteristics
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
	

#### License

Use of this dataset in publications must be cited to the following publication:

[1] Fanaee-T, Hadi, and Gama, Joao, "Event labeling combining ensemble detectors and background knowledge", Progress in Artificial Intelligence (2013): pp. 1-15, Springer Berlin Heidelberg, doi:10.1007/s13748-013-0040-3.

@article{
	year={2013},
	issn={2192-6352},
	journal={Progress in Artificial Intelligence},
	doi={10.1007/s13748-013-0040-3},
	title={Event labeling combining ensemble detectors and background knowledge},
	url={http://dx.doi.org/10.1007/s13748-013-0040-3},
	publisher={Springer Berlin Heidelberg},
	keywords={Event labeling; Event detection; Ensemble learning; Background knowledge},
	author={Fanaee-T, Hadi and Gama, Joao},
	pages={1-15}
}


### Contact

	
For further information about this dataset please contact Hadi Fanaee-T (hadi.fanaee@fe.up.pt)


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions

<div class="alert alert-block alert-success">
Final Equation of the Linear Regression Model is: </br>
\cnt = 0.385255*const + 0.224247*yr + 0.046505*workingday + (-0.251472*hum) + (-0.136941*windspeed) + (-0.139546*Spring) + 0.086837*winter + (-0.066279*Dec) + (-0.079521*Nov) + 0.065155*Sep + (-0.196867*Snow) + 0.058043*Sat
</div>

<div class="alert alert-block alert-info">
<b>After the equation we can conclude that</b> </br>

<b> yr </b>: Change in one unit of yr changes 0.224247 units of cnt assuming that all the other variable states constant </br>

<b> workingday </b>: Change in one unit of workingday changes 0.046505 units of cnt assuming that all the other variable states constant </br>

<b> atemp </b>: Change in one unit of atemp changes 0.425314 units of cnt assuming that all the other variable states constant </br>

<b> hum </b>: Change in one unit of hum changes -0.251472 units of cnt assuming that all the other variable states constant </br>

<b> windspeed </b>: Change in one unit of windspeed changes -0.136941 units of cnt assuming that all the other variable states constant </br>

<b> Spring </b>: Change in one unit of Spring changes -0.139546 units of cnt assuming that all the other variable states constant </br>

<b> Winter </b>: Change in one unit of Winter changes 00.86837 units of cnt assuming that all the other variable states constant </br>

<b> Dec </b>: Change in one unit of Dec changes -0.066279 units of cnt assuming that all the other variable states constant </br>

<b> Nov </b>: Change in one unit of Nov changes -0.079521 units of cnt assuming that all the other variable states constant </br>

<b> Sep </b>: Change in one unit of Sep changes 0.065155 units of cnt assuming that all the other variable states constant </br>

<b> Snow </b>: Change in one unit of Snow changes -0.196867 units of cnt assuming that all the other variable states constant </br>

<b> Sat </b>: Change in one unit of Sat changes 0.058043 units of cnt assuming that all the other variable states constant </br>

</div>

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
    Pandas - version 1.3.3
    Numpy - version 1.20.3
    Matplotlib - version 3.4.3
    Seaborn - version 0.11.2
    Scikit-learn - version 1.0.1
    Statsmodel - version 0.13.1

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Contact
Created by [@98abhilash] - feel free to contact me!




<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->