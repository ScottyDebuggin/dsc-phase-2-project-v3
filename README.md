# Movie Dataset Exploration and Analysis

## Overview

This repository contains a data science project focused on exploring and analyzing various movie datasets. The main goal of this project is to provide valuable insights for movie industry stakeholders, such as production companies, directors, and investors, by answering key business questions. The analysis process is conducted through data cleaning, visualization, and various statistical methods.

## Business Understanding

The movie industry is a multi-billion-dollar business, and its stakeholders are continuously looking for ways to maximize returns on their investments. This project aims to address the following key business questions:

     1. What is the relationship between movie runtime, and popularity rating?
     
     2. What is the Return On Investment(ROI) for the top 3 commonly produced movie genres?
     
     3. What is the correlation between movie popularity rating, and number of words in the title?

By answering these questions, stakeholders can make informed decisions about which genres to invest in, how much to allocate for movie budgets, and when to release movies for maximum profit potential.


# Data Understanding and Analysis

## Source of Data

### The data used in this project comes from 6 sources:

    Dataframes:
 1.  [Box Office Mojo](https://www.boxofficemojo.com/)
 2.  [IMDB](https://www.imdb.com/)
 3.  [Rotten Tomatoes](https://www.rottentomatoes.com/)
 4.  [TheMovieDB](https://www.themoviedb.org/)
 5.  [The Numbers](https://www.the-numbers.com/)

   SQL database
 6.![movie data erd](https://raw.githubusercontent.com/learn-co-curriculum/dsc-phase-2-project-v3/main/movie_data_erd.jpeg)

## Description of Data (formatted in 'Column_Name:Description')

### The dataframes contain the following columns:

##### Index ID: Unique index identifier for each entry
##### Movie Name: Title of the movie
##### Genre: Genre(s) associated with the movie
##### Director: Director of the movie
##### Studio: Production studio responsible for the movie
##### Release Date: Theatrical release date of the movie
##### DVD Date: DVD release date of the movie
##### Production Cost: Budget allocated for the production of the movie
##### Domestic Gross: Box office revenue generated in the domestic market
##### Foreign Gross: Box office revenue generated in foreign markets
##### Worldwide Gross: Total box office revenue generated worldwide
##### Age Rating: Age-based content rating for the movie
##### Critic Review Rating: Numerical rating provided by a movie critic
##### Critic Review Date: Date when the critic review was published
##### 'Fresh' or 'Rotten' (true/false): Boolean value indicating whether the movie is considered "good" or "bad" based on critic reviews
##### Critic Synopsis: Brief summary of the critic's review
##### Critic Name: Name of the movie critic
##### Review Publisher : Organization that published the critic review
##### Original Language: Language in which the movie was originally produced
##### Total Popularity Rating: Sum of all popularity ratings for the movie
##### Total Popularity Vote Count: Total number of votes contributing to the movie's popularity rating
##### Average Popularity Rating: Average popularity rating for the movie

### The database contains the following columns:

#### Movie Info:

##### Movie ID: Unique identifier for each movie
##### Movie Name: Title of the movie
##### Genre: Genre(s) associated with the movie
##### Release Year: Year of the movie's release
##### Sequential Ordering: Order in which the movie was released in a series or franchise
##### Region: Geographical region where the movie was released
##### Language: Language(s) in which the movie was produced
##### Type: Type of movie (e.g., feature film, short film, documentary)
##### Attributes: Additional attributes or features associated with the movie
##### Original Title (true/false): Boolean value indicating whether the title is the original title of the movie
##### Total Popularity Vote Count: Total number of votes contributing to the movie's popularity rating
##### Average Popularity Rating: Average popularity rating for the movie
##### Original Movie Name: Title of the movie in its original language, if different from the primary title
##### Runtime: Duration of the movie in minutes

#### Person Info:

##### Person ID: Unique identifier for signifigant individual persons involved in the movie
##### Name: Name of the person
##### Primary Profession: Primary profession or role of the person in the movie industry
##### Role Category: Category of the person's role in the movie (e.g., actor, director, producer)
##### Job: Specific job or responsibility of the person for the movie
##### Character: Name of the character portrayed by the actor in the movie
##### Birth Year: Year of birth of the person
##### Death Year: Year of death of the person (if applicable)


# Visualizations

## ROI Per Top 3 Genres

![Total Movies by Genre](https://i.imgur.com/OUvOqzh.png)
This chart visualizes the total count for of each genre type in the datasets.

![Drama](https://i.imgur.com/kMGetLW.png)
This chart visualizes the production cost and gross profit for drama movies: ROI = 149%

![Horror](https://i.imgur.com/LI2DG81.png)
This chart visualizes the production cost and gross profit for horror movies: ROI = 233%

![Documentary](https://i.imgur.com/zHuEPRc.png)
This chart visualizes the production cost and gross profit for documentary movies: ROI = 151%

![ROI_summary](https://i.imgur.com/8CsndMY.png)
Horror movies net the largest profit margin, from the tested data.

## Movie Runtime Effect on Popularity

![Runtime Pop-Rating](https://i.imgur.com/OUvOqzh.png)
This chart visualizes the trend in movie runtime, and the effect on popularity rating.

## Words Per Title Effect on Popularity

![Words Per Title](https://i.imgur.com/YYcGFyD.png)
This visual depicts the correlation in movie popularity rating, and total words in the movie tite.


# Conclusion

These insights are valuable for movie industry stakeholders and can aid in making informed decisions across various aspects of movie production and distribution.

## Brief

After analyzing the movie datasets, the following insights can be drawn: 

     1. Horror genre offers the highest return on investment (ROI), making it the most profitable option for stakeholders. 
     2. The ideal runtime for popular movie results falls within 95-145 minutes. 
     3. Shorter titles, specifically those with just 1 word, tend to be more popular compared to longer titles.

## Final Recommendation 

To produce a popular, profitable, and successful movie, a statistically informed method for a movie producer or shareholder, would be producing a Horror film, between 95-145 minutes, with a 1 word title.