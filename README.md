# Problem Statement

This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine. In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.

In this project, you are required to do

Exploratory Data Analysis

Understanding what type content is available in different countries

If Netflix has been increasingly focusing on TV rather than movies in recent years.

Clustering similar content by matching text-based features

# Project Summary

Netflix movies and TV shows clustering is a data analysis and machine learning technique that Netflix uses to group its content into similar categories. This technique involves analyzing the various characteristics of each title, such as genre, cast, and plot, and using algorithms to identify patterns and similarities.

The aim of this project is to analyze the Netflix Dataset of movies and TV shows until 2019, sourced from the third-party search engine Flixable. The goal is to group the content into relevant clusters using NLP techniques to improve the user experience through a recommendation system.

The project followed this process:

Handling null values in the dataset.

Managing nested columns (director, cast, listed_in, country) for better visualization.

Binning the rating attribute into categories (adult, children's, family-friendly, not rated).

Performing EDA to gain insights for preventing subscriber churn.

Creating clusters using attributes like director, cast, country, genre, rating, and description. These attributes were tokenized, preprocessed, and vectorized using TF-IDF vectorizer.

Reducing the dimensionality of the dataset using PCA to improve performance.

Employing K-Means Clustering and Agglomerative Hierarchical Clustering algorithms, determining optimal cluster numbers (4 for K-Means, 2 for hierarchical clustering) through various evaluation methods.

Developing a content-based recommender system using cosine similarity matrix to provide personalized recommendations to users and reduce subscriber churn for Netflix.

This comprehensive analysis and recommendation system are expected to enhance user satisfaction, leading to improved retention rates for Netflix.

# Conclusion

# Based on the exploratory data analysis (EDA) 

Movies make up about two-thirds of Netflix content, with TV shows comprising the remaining one-third.

Adult and teen categories are prevalent on Netflix, while family-friendly content is more common in TV shows than in movies.

Indian actors dominate Netflix movies, while popular Indian actors are absent from TV shows.

Jan Suter is the most common movie director, and Ken Burns is the most common TV show director on Netflix.

The United States is the largest producer of movies and TV shows on Netflix, followed by India. Japan and South Korea have more TV shows than movies, indicating growth potential in that area.

International movies, drama, and comedy are the most popular genres on Netflix.

TV show additions on Netflix have increased since 2018, while movie additions have decreased. In 2020, fewer movies were added compared to 2019, but more TV shows were added.

October, November, and December are popular months for adding TV shows, while January, October, and November are popular for adding movies. February sees the least additions.

Movies and TV show are typically added at the beginning or middle of the month and are popularly added on weekends.

Most movies on Netflix have durations between 80 to 120 minutes, while TV shows commonly have one or two seasons.

Various countries contribute adult and teen content, with Spain producing the most adult content and Canada focusing on children and family-friendly categories.

# Based on ML Model

Implemented K-Means Clustering and Agglomerative Hierarchical Clustering, to cluster the Netflix Movies TV show dataset.

The optimal number of clusters we are getting from K-means is 4, whereas for Agglomerative Hierarchical Clustering the optimal number of clusters are found out to be 2.

We chose Silhouette Score as the evaluation metric over distortion score because it provides a more intuitive and interpretable result. Also Silhouette score is less sensitive to the shape of the clusters.

Built a Recommendation system that can help Netflix improve user experience and reduce subscriber churn by providing personalized recommendations to users based on their similarity scores.
