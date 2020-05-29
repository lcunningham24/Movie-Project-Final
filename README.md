# Film Analysis 

Flatiron School Module 1 Project

Contributors: Chibuzo Ugonabo and Lauren Cunningham 
Sources: IMDB, Box Office Mojo, TMDB

## Overview 
The objective of this project was to provide Microsoft with insights and reccomendations for entering the film industry. To analyze box office success we posed the following questions: 

    1. 
    2. 
    3. 
    4.


## Data Collection
To gather our data we used both webscraping and API calls. First, we webscraped IMDB to collect data on the Top Box Office movies from 2010-2019. From IMDB, we gathered data on title, genre, domestic box office earnings, IMDB rating and movie run time. We then webscraped Box Office Mojo to fill in worldwide box office earnings for our IMDB collection. Finally, we made an API call to gather data from TMDB on budget, release date and popularity.

Data_Collection.ipynb


## Data Cleaning & Visualization 
After we gathered all of our data, we decided to merge our dataframes and save them as csv files. 

Question 1: 
To assess which genres had the highest box office earnings, we grouped our top box office data collection by genre.



We wanted to look at profit for each genre, but we had null values in our budget column. The values were missing for low grossing films, so we decided to drop the rows with null values to get a closer look profitability. 



Question 2: 
Next, we looked at just profitability by genre to see if rating affects box office performance. 


Question 3: 
To assess the best time to release a movie, we looked at profitability by month. 


Question 4: 





## Main Findings

Mystery is the most profitable genre 
Rating does not affect box office performance 
Profitability spikes in the summer months and also a little bit right before the end of the year. This is in part due to the fact that Oscar  






## Reccomendations for Microsoft


