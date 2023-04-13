<center>
    <h1> 
        Tap into Your Taste: A Beer Recommendation System
    </h1>
</center>

### <i> Performed using multiple machine learning models and filtering techniques to accurately predict the overall rating of a beer. The Focus of this project is to create a well-established recommendation system that can predict a user's preferences using review data as well as beer data.
</i> 

#### Date: April 21, 2023
#### Author: [Sean Conlon](https://www.linkedin.com/in/seanconlon29/)

<br>

<figure>
    <p align="center">
    <img src="Illustrations/beerbackground.webp"
         alt="Beer Picture for README"
         width="800"
         height="450">
    </p>
</figure>

## Table of Contents

- [Introduction](#introduction)

- [Data Cleaning](#data-cleaning)
- [Modeling](#modeling)
- [Visualization](#visualization)
- [Conclusion](#conclusion)
- [Repository Structure](#repository-structure)

## Introduction

This project is a culmination of the skills I have learned in the Flatiron School Data Science program. Using datasets from the links provided I found a dataset containing breweries across the United States [Brewery Dataset Here](https://www.kaggle.com/code/stansilas/mapping-brewery-pubs-across-us-states/input) and a dataset containing over 1.5 million reviews of beers [Review Dataset Here](https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate). I merged the two datasets together creating a beer_df. This was then used to create a beer recommender system using multiple machine learning models and filtering techniques. The resulting dataset withheld approximately 160,000 reviews.

<br>

## Data Cleaning
Data cleaning was performed using the following steps:
1. Merging the two datasets into one dataframe labeled as beer_df.
2. Only keeping the top 50 breweries within the United States, to reduce the size of the dataset and increase the accuracy of the models. 
3. Removing any missing, unneeded duplicate values as well as outliers unnecessary for the analysis.
4. Feature engineering of columns to create new features that would be useful for the analysis as well as data visualization.

<br>


## Modeling
All models performed were using the surprise package and model tuning considering GridSearchCV as well as RandomizedSearchCV. Each model has an accuracy score that is sufficient enough to be less than half a rat off from the actual rating. These models include the Collaborative Model which prioritizes the users reviews, Item-Based Model which prioritizes each feature that was rated and combined into an Ensemble Model to very accurately predict a beer's alcohol by volume (ABV) based on the brewery the beer was from. The last model created was Location-Based which takes advantage of the latitude and longitude coordinates to provide the necessary recommentations. 

#### Collaborative-Model
This model was created in order to predict a user's rating based off of similar users ratings of certain beers. Using this information it will then provide an accurate list of 5 beers that the user will most likely enjoy. The recommendations created were for not only recommending beers, but also breweries that produce similar beers as to the ones highly-rated. 

<p>
    insert code snip of model with recommendations for user
</p> 

<br> 
    
#### Item-Based Model
In order for an Item-based model to correctly predict what a users preference would be, there must be certain features of the beers within the dataset. Luckily there were reviews on certain features of each beer rating. These included:
- Aroma
    - The smell of the beer, rated from good to bad. 
- Appearance
    - The look of the beer, taking into account the coloration as well as the label.
- Taste
    - The flavoring of the beer.
- Palate
    - This is where the carbonation, mouthfeel, alcohol profile and texture really come in.

<p>
    insert code snip of model with recommendations for user
</p> 

<br>

#### Ensemble Model
As a bonus model, this was created in order to see how a user will rate a beer based on the alcohol percentage. By many of those who avidly drink beers, they consider beers with a high to very-high alcohol percentage to be of bitter-taste and flavorless resulting in a low rating for most. 

<p>
    insert code snip of model with recommendations for user
</p> 

<br> 

#### Location-Based Model
Considering the dataset includes information about the breweries, but also their locations. I felt the need to take advantage of the coordinates provided in order to give a great recommendation not only based on beers. The model was created using help from outside sources, given that I had no prior knowledge of the haversine formula. This formula combined with the coordinates as well as some functions creates a wonderful recommendation for each user.

Each user will not only be able to see the nearest breweries based on their own coordinates, but also each breweries top 5 rated beers in order to help the user decide which brewery they would prefer. 

<p>
    insert code snip of model with recommendations for user
</p> 

<br>

## Visualization
Models that were created were for the recommendation engine, but in order to see the data we need to visualize our findings. The following visualizations were interesting parts of the analysis in which I came across during the modeling process. 

<p>
    insert visuals of cool interesting maybe even interactive visuals with the dataset
</p> 

<br>

## Conclusion
    <p>
        
    </p>

<br>


## Repository Structure

```
├── data                                    <- CSV data files
├── Notebooks                               <- Jupyter notebooks dedicated to data exploration and modeling
├── Models                                  <- Data files used in analysis
├── Collaborative-Based_Model.ipynb         <- Narrative documentation of Collaborative analysis in Jupyter notebook
├── Item-Based_Model.ipynb                  <- Narrative documentation of Item-Based analysis in Jupyter notebook
├── Location-Based_Model.ipynb              <- Narrative documentation of Location-Based analysis in Jupyter notebook
├── README.md                               <- A Overall Summary in README form of this project
├── Presentation.pdf                        <- PDF version of project presentation
```
