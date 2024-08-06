# My First Website Using Flask, Python And Python Libraries Lets see
## Project Overview
This project aims to build a recommendation system using Flask, Python, and a dataset from Kaggle. The system employs three main recommendation techniques: Popularity Based Recommender System, Collaborative Filtering Based Recommender System, and Content Based Recommender System. The final models are saved using pickle for future use.
## Dataset
The dataset used for this project is from Kaggle and includes the following files:
- **Ratings.csv**: Contains user ratings for different books.
- **User.csv**: Contains information about users.
- **Books.csv**: Contains information about books.
Additionally, for the movie recommendation system:
- **[TMDB Movie Metadata](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)**: Contains metadata for movies used in the content-based recommender system.
## Technologies Used
- **Python**: The core programming language for this project.
- **Flask**: Used to create the web application for the recommendation system.
- **Pandas**: Used for data manipulation and analysis.
- **Numpy**: Used for numerical operations.
- **Pickle**: Used to save and load the trained models.
- **Scikit-learn**: Used for implementing machine learning algorithms and calculating cosine similarity.
## Recommendation Systems
### 1. Popularity Based Recommender System
This system recommends books based on their popularity. It calculates the popularity score for each book by aggregating the ratings and recommends the top N books with the highest scores.
### 2. Collaborative Filtering Based Recommender System
This system recommends books based on the preferences of users with similar tastes. It uses techniques like user-based or item-based collaborative filtering to predict a user's rating for a book based on the ratings from similar users.
### 3. Content Based Recommender System
This system recommends movies based on the similarity of their content. It uses cosine similarity to measure the similarity between movies based on their metadata.
## Implementation Steps
### Step 1: Data Preprocessing
- Load the datasets (Ratings.csv, User.csv, and Books.csv) using Pandas.
- Clean the data by handling missing values and duplicates.
- Merge the datasets to create a unified view of user ratings and book information.
### Step 2: Popularity Based Recommender System
- Calculate the popularity score for each book.
- Recommend the top N books with the highest popularity scores.
### Step 3: Collaborative Filtering Based Recommender System
- Implement collaborative filtering using techniques such as user-based or item-based filtering.
- Train the model using the available data.
- Predict ratings for books that a user has not rated yet.
- Recommend books with the highest predicted ratings.
### Step 4: Content Based Recommender System
- Load the TMDB Movie Metadata dataset.
- Preprocess the data by extracting relevant features (e.g., genres, keywords).
- Calculate the cosine similarity between movies based on their content features.
- Recommend movies with the highest similarity scores to a given movie.
### Step 5: Saving the Model
- Use Pickle to save the trained models for future use.
- Load the models when needed to make recommendations.
