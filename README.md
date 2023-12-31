

Demonstration of NLP using the Python package NLTK. Scrapes articles from Wikipedia and assigns sentiment using nltk.sentiment.vader SentimentIntensityAnalyzer. This is done for all the declared 2024 presidential candidates, and then the results are graphed and color-coded according to party affiliation.

This model assigns a sentiment to each individual word, out of context from the words around it, between -1 and 1. Different aggregates of those results are then plotted. Further analysis will involve taking the sentiment of sentences and paragraphs as a whole, which allows the model to have more context of the words. However, for this simple demonstration, it only sees and responds to one word at a time.

The default NLTK stop words list had to be expanded to include common words on political pages like "party" and "united," which skew sentiment in the positive direction.

The difference in results between the sum, mean, and median graphs is subtle but worthwhile. Candidates with much longer articles obviously have a higher chance of having their sum score skewed in one way or another if the sentiment is consistent throughout the article. The median could be the most valuable metric to compare candidates because there are no large outliers, and the scale is more easily digestible for humans.



# Individual word sentiment analysis
![Words Graph](images/5e221266-6bcd-492f-8361-18ff515f83f5.png)


# Sentence sentiment analysis
![Sentences Graph](images/7988427d-6957-4b8b-bcd1-fa2e41bf66bd.png)


In conclusion, I don't think this tells you anything you don't already know or at least don't already have an instinct towards. At the very least, it is an interesting exercise in perhaps uncovering minor biases in these articles between the lesser-known candidates.

# Dispersion Plot
This is a dispersion graph of common words used at the inugural addresses of the last 3 presidents.

![Dispersion Plot](images/dispersion_plot_of_speeches44_45_46.png)

The similarity of Obama's and Biden's address is interesting. They are approximatly the same length and have a similar distribution of key words. Trump's speech is much shorter, and invokes these buzzwords much more frequently. Biden is the only one who used the word "democracy" and he used it 11 times and 5 times in the first 56 notable (excluding stops) words. Trump is the only one to use the word "winning".

# Sentiment analysis of inagurual speeches of the last 13 presidents (first term)

![Speech Graph](images/speech_sent_analysis.png)

If this were colored by political party, it could be more informative. You would generally expect these speeches to be positive, but Truman and Eisenhower are among the leaders in all 3 measurements. Truman took office only 8 days prior to the death of Hitler (although his inaugural address was in January). HWBush is also quite positive in general, his term and prior Vice Presidency correlating with the demise of the Soviet Union, which was addressed in his speech.

# Frequency of superlative/comparitive adjectives and superlative/comparative adverbs

![Superlative graph](images/superlative_graph.png)

Interestingly, Trump used the least amount of superlative/comparative words in his inaugural address, which contrasts my opinion of his general public demeanor.

# Graph of part of speech distribution

![pos dis graph](images/2023-07-12-125227_1183x778_scrot.png)


# P-values of various parts of speech

The below chart are the p-values of the frequency from the above chart. All of the p-values that are above 0.95 or below 0.05 are highlighted. This assumes a normal distribution of parts of speech. Some interesting trends. The p-value of NN (common nouns) is trending up over time while the p-value of NNP(proper nouns) is trending down over time. This indicates that the frequency of common nouns is increasing and proper nouns is decreasing. Are presidents being less specific in their language purposely? Or is this a trend seen across all spoken english?  

![Pos graph](images/2023-07-12-123826_2982x418_scrot.png)



