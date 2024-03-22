# Movie Recommendation System

## Introduction
This project aims to develop a movie recommendation system using the TMDB 5000 Movies Dataset. The system suggests similar movies based on their plot summary, genres, keywords, cast, and crew information.

## Data Source
The dataset used for this project consists of two files:
- `tmdb_5000_movies.csv`: Contains information about movies such as budget, genres, homepage, keywords, original language, overview, popularity, production companies, release date, revenue, runtime, spoken languages, status, tagline, title, vote average, and vote count.
- `tmdb_5000_credits.csv`: Contains information about movie credits including cast and crew.

## Data Preprocessing
1. Merging the two datasets on the movie title to create a single DataFrame.
2. Handling missing values and duplicates.
3. Parsing JSON columns (genres, keywords, cast, crew) to extract relevant information.
4. Cleaning and preprocessing text data by tokenizing, stemming, and converting to lowercase.

## Feature Engineering
1. Generating movie tags by combining plot overview, genres, keywords, cast, and crew information.
2. Converting the tags into a numerical representation using CountVectorizer.

## Similarity Calculation
1. Calculating cosine similarity between movie vectors to measure their similarity.
2. Building a recommendation function to suggest similar movies based on a given movie title.

## Recommendations
The recommendation system suggests five similar movies based on a given movie title. For example, when given the movie "Her," the system recommends "Code 46," "Veer-Zaara," "Two Girls and a Guy," "Love Letters," and "The Time Traveler's Wife."

## Future Enhancements
1. Implementing collaborative filtering algorithms such as matrix factorization and nearest neighbors.
2. Incorporating user preferences and feedback to personalize recommendations.
3. Deploying the recommendation system as a web application for real-time usage.

## Conclusion
The movie recommendation system demonstrates the use of natural language processing techniques and machine learning algorithms to provide personalized movie suggestions. By leveraging movie metadata and text analysis, the system offers valuable insights into movie similarity and enhances the user experience in discovering new movies.

## References
- TMDB 5000 Movies Dataset: [Link](https://www.kaggle.com/tmdb/tmdb-movie-metadata)
- NLTK Documentation: [Link](https://www.nltk.org/)
- Scikit-Learn Documentation: [Link](https://scikit-learn.org/)
