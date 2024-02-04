# Content-based filtering

Content-based filtering is indeed a recommendation system technique that recommends items to users based on the features or content of those items. The approach was taken because of the characteristics of the dataset.



![image](https://github.com/AnaSmola/Movies_recommender/assets/94449616/4606fe23-2667-436f-8766-0c91219f1a4f)

## Characteristics of dataset

The scrapped dataset icluded the following features:

![image](https://github.com/AnaSmola/Movies_recommender/assets/94449616/5c22da4e-027b-4335-9a66-2e77b53d027c)


## Cosine similarity metric for comparing the recommenders

The cosine similarity ranges from -1 to 1, where:

- `1` indicates perfect similarity.
- `0` indicates no similarity.
- `-1` indicates perfect dissimilarity.

## Recommender systems algorithms used in the project

## 1. TF-IDF Vectorizer


**TF-IDF (Term Frequency-Inverse Document Frequency) Vectorizer** is a text processing technique often used in content-based filtering for movie recommender systems. It converts movie descriptions or features into numerical vectors, emphasizing the importance of terms within each movie description relative to the entire movie dataset.

- **Use Case:**
  - is useful when representing movie descriptions or features as numerical vectors for content-based filtering. It helps capture the uniqueness of terms within each movie's description.
![image](https://github.com/AnaSmola/Movies_recommender/assets/94449616/fbb38d47-a5b5-456b-bce9-8a416a1b41cd)

## 2. Count Vectorizer


**Count Vectorizer** is another text processing technique used in content-based filtering. It converts movie descriptions or features into numerical vectors, counting the occurrences of each term within a movie's description.

- **Use Case:**
  -  is effective when the frequency of terms within a movie's description is essential for content-based filtering. It represents movies based on term occurrences.

![image](https://github.com/AnaSmola/Movies_recommender/assets/94449616/ad41b1b1-0ec6-4636-890a-2ed076f28aa1)


## 3. K-Nearest Neighbors (KNN)


**K-Nearest Neighbors (KNN)** in a content-based recommendation system using K-Nearest Neighbors (KNN), movies are represented by feature vectors based on their content or attributes (e.g., genres, actors, director). The similarity between items is computed using a distance metric, and recommendations are made by identifying the nearest neighbors in the feature space.

- **Use Case:**
  - is suitable when recommending items (movies) based on their content attributes. It can provide personalized recommendations by considering the features that match a user's preferences.

![image](https://github.com/AnaSmola/Movies_recommender/assets/94449616/f123986d-60e7-4a6e-8799-148f5d0c3afd)


# Conclusion

The project aimed to test three different algorithms to find a system that provides users with a list of the top 5 movies based on the highest views, votes, and similarity score. The algorithm that yielded better mean scores for a list of 5 movies, was considered the better version for implementation on the website.



![image](https://github.com/AnaSmola/Movies_recommender/assets/94449616/d2de5832-acb1-4576-a5de-4845c65ee482)



* TF-IDF might be a better choice if the importance of words in movie descriptions matters
in recommendation system, the calculations involved in TF-IDF can be more intensive,
especially as the size of the corpus (collection of movie descriptions) increases

* Count Vectorization could be a simpler and faster option if the dataset is large or if the
content of the movie descriptions is not as important

* KNN Model is flexible and interpretable and can be applied to find movies similar to a given
movie based on certain features, but it is sensitive to redundant features, may not perform
well if the dataset has high dimensionality




