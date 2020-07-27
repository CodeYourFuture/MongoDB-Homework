# Import cyf_mflix_movies_popular.json into a database on your mongodb server/atlas cluster:

If you already have this data, you can skip this step.

  - In compass, select or create the db you want to import to (e.g. sample_mflix)
  - Click '+' to create a new collection. Call it movies (or movies_popular if you already have the full movies collection from sample_mflix)
  - Menu bar: Collection -> Import Data
  - Select cyf_mflix_movies_popular.json and import

# Run queries in compass to find the following answers

## Recap of week 1

1) Which 3 movies came out in 1978

2) Which 3 movies rated as PG came out in 2001

3) Which 4 movies with a metacritic score higher than 90 came out before 1950

4) Which 3 movies with a metacritic score higher than 90 came out in the 1990s

## Deepening week 1

5) Which 3 movies from Iran have a metacritic score higher than 80

6) Which 4 movies from one of the Nordic Countries (Sweden, Norway, Finland, Iceland or Denmark) came out in 2011

## New functionality

7) Which 2 movies have included both Matt Damon and Julia Stiles in the cast

8) Which movie has won 210 awards?

9) Which movie has more than 50 "rotten" reviews on rotten tomatoes, but was nominated for two Oscars

10) What are the 3 oldest movies in the database?

11) Which are the top 3 movies according to the number of "fresh" reviews on rotten tomatoes?

## More tricky (read the documentation and figure out how to do it)

12) What happens if I try to find the 5 movies with the lowest number of "fresh" reviews on rotten tomatoes? How can I work around that

# Write express endpoints that compute and returns the answers to the following questions:

## Writing simple endpoints

13) What movies include a given actor in their cast? e.g. /filmsbyactor?actors=Tom%20Cruise

14) What movies came out in a given year (e.g. /filmsbyyear?year=1999)

15) What movies have a metacritic score in a range (e.g. /filmsbyscore?minscore=60&maxscore=80)

## Building a search object

16) What movies include any of the given actors (e.g. /filmsbyactor?actors=Tom%Cruise,Matt&20Damon)

17) Write a search endpoint that optionally combines the simple endpoints (e.g. /film/search?actors=Tom%20Cruise&minscore=80 and /film/search?year=2005&maxscore=75)

## More tricky

18) What are the different kinds of "rated" categories that exist

19) Return the titles of the movies with the top 5 metacritic scores for a given "rated" category

20) How many movies have each of the different "rated" categories

21) What are the worst 5 movies by ratio of fresh to rotten reviews on rotten tomatoes, and that have at least 20 fresh and rotten reviews combined

22) Write a paginated endpoint to see all movies

23) Write an endpoint that allows searching for keywords (a single keyword) in descriptions (and/or titles)





