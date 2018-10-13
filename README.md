# Sentiment Analysis

An important part of an opinion is its sentiment. To predict these sentiments,
we use a Yelp dataset to train an Opinion Mining model.We explore
two approaches for creating features: uni-gram bag of words model and
pre-trained embeddings. The bag of words model is based on the count of
lemmatized words in each opinion. The pre-trained embeddings are built
using the GloVe model over 2B tweets. Both models extract semantic information
from the database. Stars are assigned by users to business reviews.
We first partition these stars into positive and negative sentiment. We then
focus on predicting the sentiment of a review based on a balanced set in
terms of users, businesses, positive and negative reviews.
