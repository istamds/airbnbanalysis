## Table of Contents
* [Project Motivation](#project-motivation)
* [Installation](#installation)
* [File Descriptions](#file-descriptions)
* [Results](#results)
* [Licensing, Authors and Acknowledgements](#licensing,-authors-and-acknowledgements)

## Project Motivation
AirBnB has been growing fast in the recent years, offering property owners the possibility to earn extra income, by letting their properties (mostly short term),  without having to go over the overwhelming procedures of establishing a hosting business, or having the comitment to run it permanently.  

If you are yourself a property owner and you would like to list your apartment on AirBnB, you must be wondering where to start. This project is an attempt to answer some fundamental questions and give some first insights, using as an example the provided AirBnB dataset for the city of Boston, Massachusetts, in the USA. The analysis can be found in the provided jupyter notebook file. The questions to be answered are:
* Are there any trends or seasonality in the hosting business in Boston?
* Which neighborhoods produce more income?
* How should a property be priced? 

Ofcourse this project can be used as a basis for the analysis of datasets from other areas, if provided by AirBnB, or as a starting point to get familiar with the datasets and further investigate to answer your own questions.

The full set of files related to this project are provided by AirBnB and [Kaggle](https://www.kaggle.com/airbnb/boston).

## Installation
In order to be able to run the code, the following python libraries are required:
* pandas
* geopandas
* numpy
* sklearn
* plotly
* matplotlib
* folium

## File Descriptions
There is one notebooks provided here to demonstrate the suggested approach to answer the above questions. The notebook consists of a first part regarding data exploration and cleansing, so as the datasets can be used for the further analysis. As next, we try to answer the three questions using the pandas library, explanatory graphs and statistical modelling.  

The datasets used are: 
* Listings: including full descriptions and average review score
* Calendar, including listing id and the price and availability for that day  

More information regarding the dataset can be found in [Kaggle](https://www.kaggle.com/airbnb/boston).

## Results
The results of the analysis showed that the prices are at their lowest during the first months of the year and start increasing from April on reaching their maximum in September and October at 237 dollars. Then, they start dropping again moving towards the end of the year.
The neighborhood that produces the highest income on average is Beacon Hill, followed by East Boston, Jamaica Plan and Charlestown. 
The lasso regression model applied to predict the price of a property based on its given attributes, did not produce a highly accurate prediction. However, lasso regression is a useful tool to also do feature selection. Based on that the top attributes that help in achieving a higher price for a listing are the number of bedrooms, providing the entire property over a single room, number of bathrooms and people that can be accommodated. Some amenities that have a greate impact on price are the air conditioning, indoor fireplace and the doorman.

The findings of the analysis are also presented as a article for non technical audience. The article can be found on the following link:
https://medium.com/@ioannis.stamatakis/make-the-most-out-of-your-hosting-business-in-boston-ma-bb5152e35281


### Licensing, Authors and Acknowledgements
The jupyter notebook provided, is free to be used as needed!
The datasets are provided under the [Creative Commons CC0 1.0 Universal (CC0 1.0) "Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/) Licence.
