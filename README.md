## Naive Bayes
In this lab, we’ll use the Naive Bayes algorithm to perform sentiment analysis on tweets. Given a tweet, the model determines whether it expresses a positive or negative sentiment by leveraging word frequencies and conditional probabilities.

Steps for building a Naive Bayes classifier:

 - Clean and preprocess each tweet to remove noise, punctuation, stopwords, and apply stemming
 - Build a frequency dictionary mapping each word–label pair to its occurrence count
 - Compute prior probabilities for positive and negative classes and calculate the log prior
 - Compute the log likelihoods of each word using Laplace smoothing to handle unseen words
 - Implement a prediction function that sums the log likelihoods and log prior for new tweets
 - Evaluate model performance on a test set and analyze misclassifications
 - Identify the most positive and negative words by calculating their positive-to-negative ratios

### Results:
Our Naive Bayes classifier achieves about 99.5% accuracy on the test dataset. Positive words like “:)” and “glad” are strongly associated with positive sentiment, while words like “:(” and “lost” correspond to negative sentiment. We also explore cases where the model makes incorrect predictions and test the classifier on our own custom tweet.
