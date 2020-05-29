# Film Analysis 

Flatiron School Module 1 Project

Contributors: Chibuzo Ugonabo and Lauren Cunningham 
Sources: IMDB, Box Office Mojo, TMDB

## Overview 
The objective of this project was to provide Microsoft with insights and reccomendations for entering the film industry. To analyze box office success we posed the following questions: 

1. Which genres are most common on the IMDB Top Box Office list?
2. Which of these genres are the most profitable?
3. How does IMDB rating performance correlate with profit?
4. When is the best time to release a movie?

## Data Collection
To gather our data we used both webscraping and API calls. First, we webscraped IMDB to collect data on the Top Box Office movies from 2010-2019. From IMDB, we gathered data on title, genre, domestic box office earnings, IMDB rating and movie run time. We then webscraped Box Office Mojo to fill in worldwide box office earnings for our IMDB collection. Finally, we made an API call to gather data from TMDB on budget, release date and popularity.

Data_Collection.ipynb


## Data Cleaning & Visualization 
After we gathered all of our data, we decided to merge our dataframes and save them as csv files. 

Question 1: 

To assess which genres were most common, we grouped our top box office data collection by genre.

See: fig2.png

Question 2

We wanted to look at profit for each genre, but we had null values in our budget column. The values were missing for low grossing films, so we decided to drop the rows with null values to get a closer look profitability. 

See: fig_profitgenre.png, fig_revenuebudgetprofit.png

Question 3: 

Next, we looked at just profitability by genre to see if rating affects box office performance. 

See: fig_profitratings.png

Question 4: 

To assess the best time to release a movie, we looked at profitability by month. 

See: fig_months.png

## Main Findings

1. Mystery is the most profitable genre
2. Profit and ratings are not necssarily correlated 
3. Profitability spikes in June, November and December 


## Recommendations for Microsoft

Mystery is the most profitable genre but because a movie can have more than one genre, we recommend that you produce movies included the top 10 genres: Mystery, Music, SciFi, Adventure, Animation, Fantasy, Action, Musical, Family, Biography. 

Ratings are not an important factor to consider, as they are not a strong indicator of a successful movie. We recommend focusing on other variables. 

Lastly, we recommend that Microsoft keep in mind this timeline and release movies accordingly. 