# SentimentAnalysisUsingBert

Sentiment Analysis is a major task in Natural Language Processing (NLP) field. It is used to understand the sentiments of the customer/people for products, movies, and other such things, whether they feel positive, negative, or neutral about it. It helps companies and other related entities to know about their products/services and helps them to work on the feedback to further improve it.

We will be using the IMBD dataset, which is a movie reviews dataset containing 100000 reviews consisting of two classes, positive and negative.

The model will take around two hours on GPU to complete training, with just 1 epoch we can achieve over 93% accuracy on validation, you can further increase the epochs and play with other parameters to improve the accuracy.

tokenizer. encode will encode our test example into integers using Bert tokenizer, then we use predict method on the encoded input to get our predictions. The model. predict will return logits, on which we can apply softmax function to get the probabilities for each class, and then using TensorFlow argmax function we can get the class with the highest probability and map it to text labels (positive or negative).
