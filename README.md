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
- [Visualization](#visualization)]
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
    <p>
        
    </p>

<br>

## Visualization
    <p>
        
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
