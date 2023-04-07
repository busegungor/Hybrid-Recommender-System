# Hybrid Recommender System

## Collaborative Filtering
While item-based collaborative filtering and user-based collaborative filtering are referred to as memory-based in the literature, model-based collaborative filtering is referred to as the latent factor model.

### Item Based Collaborative Filtering
Recommendations are made based on item similarity. For example, a film similar to the liking features of a watched film is recommended. It has no relation to content similarity. I want to make a decision according to the consensus of the community.

### User Based Collaborative Filtering 
Recommendations are made based on user similarities. Let's say I watched a movie and liked it. Others also watched the same movie and liked it. Then I want to watch another movie. They recommend me the other movie that people who liked the movie I liked also liked. In other methods, we were only interested in a person's contact with other films.


![image](https://user-images.githubusercontent.com/64617036/230678467-8177f998-ddc8-44f2-a70a-bed40e8bf3aa.png)

## Business Problem
Use item-based and user-based recommender methods to make predictions for the user with the given ID. Consider 5 recommendations from the user-based model and 5 recommendations from the item-based model and make a total of 10 recommendations from 2 models.

![image](https://user-images.githubusercontent.com/64617036/230678611-05227c21-00ad-45b9-a418-ac9c0e8f4603.png)

## About Dataset
* Content

The Book-Crossing dataset comprises 3 files.

* Users

Contains the users. Note that user IDs (User-ID) have been anonymized and map to integers. Demographic data is provided (Location, Age) if available. Otherwise, these fields contain NULL-values.

* Books

Books are identified by their respective ISBN. Invalid ISBNs have already been removed from the dataset. Moreover, some content-based information is given (Book-Title, Book-Author, Year-Of-Publication, Publisher), obtained from Amazon Web Services. Note that in case of several authors, only the first is provided. URLs linking to cover images are also given, appearing in three different flavours (Image-URL-S, Image-URL-M, Image-URL-L), i.e., small, medium, large. These URLs point to the Amazon web site.

* Ratings

Contains the book rating information. Ratings (Book-Rating) are either explicit, expressed on a scale from 1-10 (higher values denoting higher appreciation), or implicit, expressed by 0.

https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset?select=Users.csv
