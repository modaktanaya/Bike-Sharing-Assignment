# Bike-Sharing-Assignment
> You are required to model(Multiple Linear Regression) the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information
Boombikes is a bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

The company wants to know:

Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demands
Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.
To get this insights, we will build a model to represent the demand for shared bikes with the available independent variables.

## Technologies Used
- Pandas Library
- Numpy Library
- Matplotlib Library
- Seaborn Library
- Statsmodels Library
- Scikit-Learn Library

## Conclusions

We carried out this Multiple Linear Regression model using the mixed approach. We first created the model with manually selecting all the independent variables. There we encountered the high p values, so we then used the RFE(Recursive Feature Elimination) method to select the top 15 features from our bikes data. Further we built the model with those selected features. We checked for the p values and VIFs for independent variables, all the p values were less than 0.05 and VIFs less than 5. 
After that, we built the final model with those 15 features and it explains the 84% variance of the training data and 80% variance of the testing data.

- We have normalized the continuous variables and all the categorical variables are now the dummy variables with level (n-1), so we have the scale of minimum=0, maximum=1 for all the variables.
- Upon normalizing the values of the predictor variables i.e. the independent variables, from the above chart, we can say that features influencing the number of rental bikes are ````temp````, ````2019```` and ````Light Snow/Rain```` followed by ````windspeed```` and ````humidity````.
- The demand of bikes rises significantly with the rising temperature, if the year is 2019 and decreases when the weather is little snowy or rainy or windspeed rises.

The final model shows the following relationship between the predictor and target variable : 

````count```` = 2132.262 - 2075.683````Light Rain/Snow```` - 1455.884````humidity```` - 1694.925````windspeed```` - 348.112````Jan```` - 372.446````July```` - 368.222````Sun```` - 461.772````Cloudy/Misty```` + 661.138````summer```` + 373.288````May```` + 778.666````Sept```` + 1090.801````winter```` +  1994.410````2019```` + 4963.951````temp````

## Acknowledgements
Give credit here.
- This project is developed as part of Linear Regression Assignment module, Master of Machine Learning and AI, IIIT-Bangalore.


## Contact
Created by [@modaktanaya] - feel free to contact me!
