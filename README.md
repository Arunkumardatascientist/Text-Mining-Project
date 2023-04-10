# Text-Mining-Project
To classify the sentiment of people about the product whether it is positive or negative using Text Analytics, including text extraction, cleaning, pattern identifications


This article was published as a part of the Data Science Blogathon

Introduction
Natural Language processing, a sub-field of machine learning has gained immense popularity in the last 5 years in both research and industrial applications due to the advancement in the field of deep learning and improvement in the computational power of hardware systems. It is a technique for computers to understand how human languages work involving the usage of computational linguistics and the computer science domain. In recent years, NLP has found its usage in several applications related to understanding and interpreting text, audio, and video files.

Sentiment Analysis
One of the key areas where NLP has been predominantly used is Sentiment analysis. The understanding of customer behavior and needs on a company’s products and services is vital for organizations. Generally, the feedback provided by a customer on a product can be categorized into Positive, Negative, and Neutral. Interpreting customer feedback through product reviews helps companies evaluate how satisfied the customers are with their products/services.

![image](https://user-images.githubusercontent.com/114068300/230829942-df3d07f5-8f8f-45ef-8b50-90f54e7abe74.png)

NLTK
For performing sentiment analysis, we will use NLTK package of the Python. Christopher Manning says, “NLTK is sort of the Swiss Army Knife of NLP meaning that it’s not terribly good for anything. But it has a lot of basic tools.” For accessing Wordnet, it’s an easy solution.

Wordnet
WordNet is a large lexical database of English developed by the Princeton University. Nouns, verbs, adjectives and adverbs are grouped into sets of cognitive synonyms (synsets), each expressing a distinct concept. Synsets are interlinked by means of conceptual-semantic and lexical relations (Fellbaum, 1998). In other words, Wordnet can be described as online thesaurus. It tells you about word meanings and relationships between word meanings. Wordnet was first created in 1985, and still in improvement.

Wordnet can be obtained by:

import nltk
nltk.download('wordnet')
In this study, we will use two main sentiment classifiers:

1. Polarity

2. Subjectivity

The TextBlob package for Python is a convenient way to perform sentiment analysis. When calculating sentiment for a single word, TextBlob takes average for the entire text. For heteronym words, Textblob does not negotiate with different meanings. In the other words, only the most common meaning of a word in entire text is taken into consideration. For making all these modelling, Textblob uses WordNet Database.

Polarity
Polarity is float which lies in the range of [-1,1] where 1 means positive statement and -1 means a negative statement. Figure 1 shows the distribution of polarity score in reviews. Most of the reviews are on positive side of the plot 
