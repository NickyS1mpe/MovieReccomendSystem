# Movie_reccomend_system

Movie Recommend System Using SVD

# Conclusion

The Movie Recommendations Homework involved the analysis and recommendation of movies based on the MovieLens dataset. The key steps and findings are summarized below:

## Overview:

This homework provides insights into collaborative filtering using SVD, cosine similarity, and personalized movie recommendations based on user behavior.

1. **Data Loading and Analysis:**
   - Three datasets (ratings, movies, users) were loaded and merged to form a comprehensive dataset.
   - A pivot table was created to find the mean ratings for each movie, and the top-rated movies were identified.

2. **Ratings Matrix Creation:**
   - A ratings matrix was created using NumPy to represent user ratings for movies.
   - Three users who rated "Batman Returns" (MovieID 1377) were selected for later comparison.

3. **Normalization:**
   - Z-score normalization was performed on the ratings matrix.
   - Missing values were replaced with the mean ratings for each movie.

4. **Singular Value Decomposition (SVD):**
   - SVD was applied to the normalized ratings matrix, resulting in U, S, and VT matrices.
   - Reconstructed matrices Rk were generated for k values of 100, 1000, 2000, and 3000.

5. **Prediction Comparison:**
   - Original and predicted ratings for the selected users on "Batman Returns" were compared for different ranks.

6. **Cosine Similarity:**
   - Cosine similarity was computed based on the rank-1000 reconstructed ratings matrix.
   - Top similar movies to "Batman Returns" were identified using cosine similarity.

7. **Movie Recommendations:**
   - User similarity was determined, and movie recommendations were provided for a specific user (ID 5954).
   - Recommendations were based on movies highly rated by a similar user but not yet seen by the target user.
