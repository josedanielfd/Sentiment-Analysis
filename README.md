# Sentiment Analysis

Introduction:
An important part of an opinion is its sentiment. To predict these sentiments, we use a Yelp dataset to train an Opinion Mining model.We explore two approaches for creating features: uni-gram bag of words model and pre-trained embeddings. The bag of words model is based on the count of lemmatized words in each opinion. 

The pre-trained embeddings are built using the GloVe model over 2B tweets. Both models extract semantic information from the database. Stars are assigned by users to business reviews.

We first partition these stars into positive and negative sentiment. We then focus on predicting the sentiment of a review based on a balanced set in terms of users, businesses, positive and negative reviews.


Dataset:
The dataset we will use for training our general review sentiment model is made available by Yelp for the Yelp Challenge. This challenge’ objective is that students use their data in innovative ways and break ground in research. The dataset consists of 7 JSON files with information about businesses (business id, location, name, category, business hours, and business attributes), users (user check-in, stars given by a user to a business, review, review date), and user’s friends.

Of these JSON files, we use the dataset containing the reviews, with the following variables: user id, business id, stars, and reviews. It has 5.2 million data points.

The Dataset can be found at: https://www.yelp.com/dataset/challenge
