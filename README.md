# Mid-Bootcamp Project
# EUR/h - A Price Calculator for second Hand Cars

## Introduction

The purpose of this project is to predict the price of your car based on the data collected from a website dedicated to selling second hand cars.

The Website: https://www.standvirtual.com/

## The Code:

### WebScraping:

First we have the web scraping part.

In the website, we go through the different parts of the html code and extract the different cars info.

I got Car Price, Car Full Name (Brand and Model), Car Km, Car Registration Year and the link for a picture.

The website does not allow us to get the full 44.000 cars. I end up with several duplicate cars.

After cleaning, we get a sample of those 44.000. For price prediction purposes, this sample is sufficient.


### Data Frame Cleaning:

In this part of the code we clean the main DF and get new columns, like car brand and car model. we also get a new DF with CITROEN C3 and AUDI A1 cars. I also get a DF with VW Polo and RENAULT Clio for comparison. 


### Data Frame EDA:

I analysed the data with C3 and A1 models. Get price evolution regarding Km and car age. Later i got the depreciation of the price of the car by age and i compare if the brand has some impact (Citroen, Audi, VW and Renault).


### Hypothesis Testing:

Null-hypothesis - Km range has no influence on car price (Yes or No?)


### Prediction Models:

I separated the DF in to AUDI and CITROEN and built 4 different models - Linear Regression, KNN Regressor, Random Forest and ADR Model. We can see with one is more effective.


### Price Calculator:

After the model analysis, i choose Random Forest and Linear Regression has the most effective models and make a calculator with user input that gives the current market price and the future price for the next five years - Works only if your car is a Citroen C3. (Its going to do all brands and models in the future)