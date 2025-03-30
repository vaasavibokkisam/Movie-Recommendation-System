# Movie-Recommendation-System
![image alt](https://github.com/vaasavibokkisam/Movie-Recommendation-System/blob/main/Screenshot%202025-03-30%20233825.png?raw=true)
# Business Objectives :
The goal of this project is to enhance user experience by providing personalized movie recommendations based on their preferences. Instead of users manually searching for movies, the system suggests similar movies using content-based filtering.
# Data Collection :
The dataset has been obtained from Grouplens.
Link:https://drive.google.com/file/d/1cCkwiVv4mgfl20ntgY3n4yApcWqqZQe6/view
# Modelling :

 Steps in the Modeling Process
1. Feature Extraction (TF-IDF Vectorization)

We extract meaningful features from text-based attributes like genres, keywords, tagline, cast, and director.

We use TF-IDF (Term Frequency-Inverse Document Frequency) to convert text data into numerical form.

Why TF-IDF? It reduces the impact of common words and highlights unique terms that define a movie.

2. Similarity Calculation (Cosine Similarity)

We compute cosine similarity between movie feature vectors.

Cosine similarity measures how close two movies are in the feature space.

The higher the similarity score, the more relevant the recommendation.

3. Finding Similar Movies

The user inputs a movie name.

We use difflib.get_close_matches() to handle spelling variations and find the best match.

Once the closest match is found, we retrieve the top 30 movies with the highest similarity scores.

4. Sorting & Ranking Recommendations

We sort the similar movies based on their similarity scores in descending order.

The top results are presented as recommendations.
# Result :



