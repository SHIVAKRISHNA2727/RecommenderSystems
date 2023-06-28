# RecommenderSystems

Recommender Systems with Python

Welcome to the code notebook for Recommender Systems with Python. In this tutorial, we will create basic recommendation systems using Python and pandas. Please note that there is another notebook called "Advanced Recommender Systems with Python" that delves into more detailed concepts using the same dataset.

In this notebook, we will focus on building a basic recommendation system that suggests items similar to a specific movie, based on user ratings. However, it is important to understand that this is not a fully robust recommendation system. It simply provides information about movies/items that are most similar to your selected choice.

We won't be working on a specific project for this topic, but you have the option to explore the advanced lecture version of this notebook (totally optional!).

Let's get started!

1. Importing Libraries:
We begin by importing the necessary libraries, including numpy and pandas, which will be used for data manipulation and analysis.

2. Getting the Data:
We read the dataset from a file called "u.data", which contains information about user ratings for different movies. The dataset is loaded into a pandas DataFrame with columns representing user ID, item ID (movie ID), rating, and timestamp.

3. Movie Titles:
Next, we load the movie titles from a file called "Movie_Id_Titles" into another DataFrame. This file contains the mapping of item IDs to movie titles.

4. Data Exploration and Analysis:
We perform exploratory data analysis (EDA) to gain insights into the dataset. We calculate the average rating and number of ratings for each movie, and create a ratings DataFrame. We also visualize histograms and a joint plot to understand the distribution of ratings and number of ratings.

5. Building the Recommendation System:
We move on to creating a simple recommendation system. We start by creating a matrix where rows represent user IDs and columns represent movie titles. Each cell in the matrix contains the rating given by a user for a particular movie. NaN values indicate movies that haven't been rated by users.

6. Recommending Similar Movies:
To recommend similar movies, we calculate the correlation between user ratings for a chosen movie (e.g., "Star Wars (1977)") and all other movies. We also calculate the correlation for the movie "Liar Liar (1997)". These correlations help us identify movies that are most similar to the chosen movie based on user ratings.

7. Refining the Recommendations:
We refine the recommendations by filtering out movies with fewer than 100 ratings. This ensures that we consider only movies with a sufficient number of ratings for a more accurate correlation analysis. We then sort the correlated movies by their correlation values and present the top recommendations.

That's it! This code provides a basic understanding of how recommendation systems work using collaborative filtering and correlation analysis.
