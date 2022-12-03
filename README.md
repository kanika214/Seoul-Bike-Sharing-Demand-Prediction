<h1 align="center"> Seoul Bike Sharing Demand Prediction </h1>
<h3 align="center"> AlmaBetter Verfied Project - <a href="https://www.almabetter.com/"> AlmaBetter School </a> </h5>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
<p align="center"> 
<img src="https://user-images.githubusercontent.com/18574968/205460839-c3e47346-a00f-438a-989d-2084bf5bd91b.jpeg" align = 'center' height='400'>
</p>

## 📋 Summary

Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes. People use bike-share for various reasons. Some who would otherwise use their own bicycle have concerns about theft or vandalism, parking or storage, and maintenance. The typical bike-share has several defining characteristics and features, including station-based bikes and payment systems, membership and pass fees, and per-hour usage fees.A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.Which variables are significant in predicting the demand for shared bikes. How well those variables describe the bike demands Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the Seoul based on some factors.

# Business/Market Goal:
You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.

Project Objectives
To highlight the main variables/factors influencing rental bike count.
To predict bike count required at each hour for the stable supply of rental bikes.
To compare the various machine learning models and find out best model for the above task.

### Attribute Information:

* Date : year-month-day
* Rented Bike count - Count of bikes rented at each hour
* Hour - Hour of he day
* Temperature-Temperature in Celsius
* Humidity - %
* Windspeed - m/s
* Visibility - 10m
* Dew point temperature - Celsius
* Solar radiation - MJ/m2
* Rainfall - mm
* Snowfall - cm
* Seasons - Winter, Spring, Summer, Autumn
* Holiday - Holiday/No holiday
* Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)

## Steps involved

o	Reading and understanding data\
o	Data cleaning\
o	Exploratory Data Analysis(EDA)\
o	Data Visualization\
o	univariate Analysis\
o	Outliers’ detection\
o OLS model Building
o	VIF (variance inflation factor) values calculation.

## Feature engineering

We have extracted month and year from the date column. To select the most relevant features we have used correlation matrix and VIF to remove multi-collinear features. We have also dropped some features like rainfall and snowfall which contain most of the zero values and also these features are slightly correlated with the dependent variable.

## List of models

* Linear Regression
* Regularized Linear Regression
   o Lasso regression and 
   o Ridge regression

## Conclusion
Linear as well as ridge Regression is giving the best score of our model with 80% accuracy.

• Outliers of numerical columns have been treated by trimming method but outliers of categorical columns have been left as they are because we cant define classed outliers.

• The outliers of Dependent variable are transformed because they can't be changed.

• Evalaution matrix shows that there is minimum error in this model.

However, this is not the ultimate end. As this data is time dependent, the values for variables like temperature, windspeed, solar radiation etc., will not always be consistent. Therefore, there will be scenarios where the model might not perform well. As Machine learning is an exponentially evolving field, we will have to be prepared for all contingencies and also keep checking our model from time to time. Therefore, having a quality knowledge and keeping pace with the ever evolving ML field would surely help one to stay a step ahead in future.


