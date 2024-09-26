# Movie Recommendation System

This repository contains the implementation of a Movie Recommendation System using two popular recommendation techniques:
1. **Content-Based Filtering** using cosine similarity
2. **Collaborative Filtering** using Singular Value Decomposition (SVD)

The system uses a dataset of movie ratings to recommend movies to users based on their preferences.

## Dataset

The dataset used in this project is a collection of movie ratings by different users. It includes genres associated with each movie which is utilized for content-based filtering, and user ratings for collaborative filtering.

## Content-Based Filtering

### Implementation Details
- **Data Preprocessing:** The genres of the movies are extracted and converted into a format suitable for cosine similarity calculation.
- **Cosine Similarity:** The cosine similarity between movies based on genres is computed to find movies similar to a given movie.

### Steps to Run
1. Load the movie data with genres.
2. Clean and preprocess the data to get genre vectors for each movie.
3. Calculate the cosine similarity between movies.
4. Use the similarity scores to find and suggest movies similar to a given movie.

## Collaborative Filtering

### Implementation Details
- **User-Item Matrix:** A matrix is created where rows represent users and columns represent movies. The entries of this matrix are the ratings given by users to movies.
- **Matrix Factorization using SVD:** Singular Value Decomposition (SVD) is applied to the user-item matrix to capture latent factors associated with users and movies.
- **Recommendations:** Based on the latent features, the system predicts ratings for movies not yet rated by a user and suggests movies with the highest predicted ratings.

### Steps to Run
1. Load the user ratings data.
2. Construct the user-item matrix.
3. Apply SVD to decompose the matrix.
4. Predict ratings for movies the user hasn't rated.
5. Recommend movies with the highest predicted ratings.

## Requirements

- Python 3.x
- Libraries: pandas, numpy, scikit-learn

## Setup and Installation

```bash
pip install pandas numpy scikit-learn
