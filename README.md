# MovieRecommender2
## Project Proposal
A theoretical streaming service wants to create an algorithm for recommending new films to their customers. In this scenario, we assume that the streaming service has a rating system on a scale from 0 to 5. To create this recommendation system, I will use a K-Nearest Neighbors model. This model will identify the viewers with similar tastes to a given user, then uses the average ratings of those similar users to predict what the target user will rate highly

## Data Source: 
We will use the MovieLens Small Dataset (https://grouplens.org/datasets/movielens/)

## Technology
We will use Python with the Pandas and NumPy libraries

## Concepts
We can think of each user as being a point in an imaginary space, where rather than having 3 dimensions, this space is N-dimensional, ("N" is the number of movies in the dataset). Each "direction" in this space represents the rating the user has given a particular movie. To identify users with similar tastes, we find the distance between users in a method equivalent to finding the distance between two points on a flat plane. Once we have identified the "nearest neighbors" (the users with a taste profile similar to the subject user), we find what movies those neighbors have rated which the subject has not yet seen. We then average the neigbors' ratings to create a prediction for what rating the user will give.

In non-technical terms, the core idea is that people who have enjoyed similar movies in the past will likely enjoy other movies that similar users enjoyed, thus we identify similar users and use their ratings to predict what a given user will rate a movie they haven't seen yet.
