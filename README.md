# Bike-Sharing-Assignment
## Bike-Sharing-Case-Study-Notebooks Problem Statement

A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

Which variables are significant in predicting the demand for shared bikes. How well those variables describe the bike demands Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.

## Business Goal: 
You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.

## Conclusion:
## We can see the demand for bikes depends mainly on below variables:
### spring , summer , December , January , November , September , Light rain_Light snow_Thunderstorm , Mist_cloudy , yr , holiday , windspeed
1. Summer is followed by Spring, which is to be expected given that the 
weather is ideal for motorcycling.
2. 2019 had a higher median than 2018, which may be due to the growing 
popularity of bike rentals and people's greater environmental consciousness. 
Median bike rentals are increasing year over year.
3. Because fall months have a larger median, the overall spread in the
month plot reflects the season plot.
4. On days other than holidays, people rent more frequently, 
which could indicate that they prefer to utilize their own 
automobiles and spend time with their families over renting 
bikes on holidays.
5. While the overall median for all days is the same, the spread on
Friday and Monday is larger, as may be seen.
6. The median for working and non-working days is about the same,
but the dispersion is larger on non-working days since some people
may have plans and not wish to rent bicycles on those days.
7. Because they are temperate, have minimal humidity, and are 
cooler in temperature, clear sky are great for renting bikes.

## Libraries Used:
### For analysis and numerical functions
import pandas as pd
import numpy as np
### For Vizualization
import seaborn as sns
import matplotlib.pyplot as plt
### Extra
import warnings
warnings.filterwarnings(action='ignore')
### For modelling
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import MinMaxScaler
from sklearn.feature_selection import RFE
from sklearn.linear_model import LinearRegression
from statsmodels.stats.outliers_influence import variance_inflation_factor
import statsmodels.api as sm
from sklearn.metrics import r2_score
