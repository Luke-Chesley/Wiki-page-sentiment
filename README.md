

Demonstration of NLP using the Python package NLTK. Scrapes articles from Wikipedia and assigns sentiment using nltk.sentiment.vader SentimentIntensityAnalyzer. This is done for all the declared 2024 presidential candidates, and then the results are graphed and color-coded according to party affiliation.

This model assigns a sentiment to each individual word, out of context from the words around it, between -1 and 1. Different aggregates of those results are then plotted. Further analysis will involve taking the sentiment of sentences and paragraphs as a whole, which allows the model to have more context of the words. However, for this simple demonstration, it only sees and responds to one word at a time.

The default NLTK stop words list had to be expanded to include common words on political pages like "party" and "united," which skew sentiment in the positive direction.

The difference in results between the sum, mean, and median graphs is subtle but worthwhile. Candidates with much longer articles obviously have a higher chance of having their sum score skewed in one way or another if the sentiment is consistent throughout the article. The median could be the most valuable metric to compare candidates because there are no large outliers, and the scale is more easily digestible for humans.

In conclusion, I don't think this tells you anything you don't already know or at least don't already have an instinct towards. At the very least, it is an interesting exercise in perhaps uncovering minor biases in these articles between the lesser-known candidates.



![sum_sen_score](https://github.com/Luke-Chesley/Wiki-page-sentiment/assets/106439301/22868546-db42-4e0f-ba28-2ba0e3af7c35)

![mean_sen_score](https://github.com/Luke-Chesley/Wiki-page-sentiment/assets/106439301/bfe55bce-cbee-4c37-8c0e-56b8f6fc8178)

![median_sen_score](https://github.com/Luke-Chesley/Wiki-page-sentiment/assets/106439301/fbc370a1-401c-4840-b7b6-49ed26dd1228)


