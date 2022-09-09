# Data_Scientist_Blog_Post

This project is part of my Data Sciene Nanodegree project by Udacity.

## Libraries
The developer needs to import the following libraries to run the analysis:
- numpy 
- pandas 
- matplotlib
- sklearn
- seaborn 
- datetime

## Motivation for project
When looking at different dataset for that project, the AirBnB dataset caught my attention since I personally often use it when being on vacation - and I even used AirBnB when spending time in Seattle.

The following three business questions motivated me to proceed with my analysis:

1. Which features are associated with higher prices?
2. Is it possible to predict the prices based on the given features?
3. How did the availability by property type develop over time?

The goal of my analysis is to eventually provide insights for both hosts and travelers active on AirBnB.

## Dataset
The analysis uses the open dataset [Seattle AirBnB 2016](https://www.kaggle.com/datasets/airbnb/seattle) provided by Keggle. It includes the following three files.

- **listings.csv**: full descriptions and average review score
- **reviews.csv**: unique id for each reviewer and detailed comments
- **calendar.csv**: including listing id and the price and availability for that day

The data cover a date range between 01/04/2016 and 01/02/2017 and include 84849 unique listings. 

## Result summary

- I found out that there are a few features that significantly drive the price, mainly related to the size of the apartment.
- Pricing is not arbitrary, and I can build a model that reproduces the pricing based on selected features as well as predicts pricing reasonably. Feel free to feed my model with your idea of a nice stay and you will get a price!
- Apartment availabilities do not show clear seasonality but the data recommend to travel off-season.

Please check out my [notebook](https://github.com/nikextens/Data_Scientist_Blog_Post/blob/main/Udacity_Data_Scientist_Project1.ipynb) for the detailed findings!

My research is not without limitations. The findings here are observational, not the result of a formal study. 
- Depending on your priorities when staying abroad the potentially relevant features might change. 
- Furthermore, I applied a rather simple model and did not compare its performance with other models. It only makes sense to also use additional models on top of linear regression to predict prices (e.g., random forest or voting ensemble).
- The data also includes various categorical variables that include continuous text in form of comments. Given that, the analysis would benefit from introducing Natural Language Processing (NLP). NLP could process the comments and convert them, e.g., into a numerical sentiment.

## Acknowledgments
Although the data are provided by Keggle, they are part of Airbnb Inside, and the original source can be found [here](http://insideairbnb.com/get-the-data/).
