

Demonstration of NLP using python package NLTK. Scrapes articles from wikipedia and assigns a sentiment using nltk.sentiment.vader SentimentIntensityAnalyzer. This is done for all the declared 2024 presidential candidates, then the results are graphed and color coded acccording to party affilation. 

This model assignes a sentiment to each individual word, out of context from the words around it, between -1 and 1. Different aggregates of those results are then plotted. Further analysis will involve taking the sentiment of sentences and paragraphs as a whole, which allows the model to have more context of the words, but for this simple demonstration it only sees and responds to one word at a time.

The default nltk stop words list had to be expanded and include common words on political pages like "party", and "united" which skew sentiment in the positive direction.

The difference in results between the sum,mean and median graphs is subtle but worthwhile. Candidates with much longer articles obviously have a higher chance of being skewed in one way or another if the sentiment is consistent throughout the article. 


![sum_sen_score](https://github.com/Luke-Chesley/Wiki-page-sentiment/assets/106439301/22868546-db42-4e0f-ba28-2ba0e3af7c35)

![mean_sen_score](https://github.com/Luke-Chesley/Wiki-page-sentiment/assets/106439301/bfe55bce-cbee-4c37-8c0e-56b8f6fc8178)

![median_sen_score](https://github.com/Luke-Chesley/Wiki-page-sentiment/assets/106439301/fbc370a1-401c-4840-b7b6-49ed26dd1228)


