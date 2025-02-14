# Movie Recommendation with Probabilistic Approach - Bayesian Network

## Overview

The project aims to propose an movie recommendation system using a probabilistic framework based on Bayesian Networks. By considering various factors like user preferences, movie genres, ratings, and other conditional relationships, this system can offer personalized recommendations that maximize user satisfaction.

**Dataset used**: [MovieLens 1M](https://grouplens.org/datasets/movielens/1m/).

## Idea

**The idea**: "*Given the rated movies, What is the probability of movie M getting rated as R?*"

$$
P(A|B) = \frac{P(B|A) P(A)}{P(B)}
$$

**The problem**: "*How to construct such a Bayesian network? What are the variables? and How do they depend on each other?*"

**The proposal**: Based on the idea of content-based filtering - "*People like similar items*", we can say similar items, or movies from the same genre affect the probability of each others. And since one genre contains many movies and one movies may belong to many genres, the Bayesian network might look like this:

![Bayesian network](./img/Bayesian%20Network.JPG)