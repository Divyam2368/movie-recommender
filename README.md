# Movie Recommender System

A content-based movie recommendation system that suggests similar movies based on user selection.

## Overview

This project implements a movie recommendation system using content-based filtering. The system analyzes movie features such as genres, keywords, cast, and crew to calculate similarities between movies and recommend similar titles.

## Features

- Select from thousands of movies in the TMDB database
- Get personalized movie recommendations based on your selection
- View movie posters fetched from the TMDB API
- User-friendly interface built with Streamlit

## Tech Stack

- **Python**: Core programming language
- **Pandas**: Data manipulation and analysis
- **Scikit-learn**: Machine learning algorithms (CountVectorizer and Cosine Similarity)
- **Streamlit**: Web application framework
- **TMDB API**: For fetching movie posters and additional information

## Project Structure

- `app.py`: Main Streamlit application
- `recommender.py`: Script that processes movie data and creates similarity model
- `movie_list.pkl`: Pickled DataFrame containing movie information
- `similarity.pkl`: Pickled matrix of cosine similarities between movies

## How It Works

1. Movie data is preprocessed to extract important features
2. Text data is vectorized using CountVectorizer
3. Cosine similarity is calculated between all movies
4. When a user selects a movie, the system finds the most similar movies
5. Movie posters are fetched from TMDB API
6. Recommendations are displayed in the Streamlit interface
