# Kuria's Data Science Portfolio
# [Project 1: BigMart Outlet Sales Prediction](https://github.com/KuriaDan/Data-Science-Projects/tree/master/Big_Mart_Sales_Prediction)


* Created a model that estimates sales for an outlet of a big chain based on a datathon hosted by [Analytics Vidhya](https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/#ProblemStatement).
* Did EDA and data cleaning.
* Explored different methods of categorical encoding, from LabeEncoding, OneHotEncoding, mean Encoding to Catboost's implementation of the same to find the optimal way of dealing with categorical variables.
* Created a baseline Catboost model That was used to gauge the performance of a more advanced approach.
* Used diverse models in creating the final model in a 1 layer stacking using SKlearn's StackingRegressor.
* Averaged the models to get the best score.
  
![alt text](https://github.com/KuriaDan/Data-Science-Projects/blob/master/Big_Mart_Sales_Prediction/images/ds_p.PNG 'model architecture')


***
# [Project 2. Text Summarizer Flask Web App](https://github.com/KuriaDan/Data-Science-Projects/tree/master/Text_summarizer)

With the death of jounalism and the incentivization of clickbait by the prevailing ad model, it's hard to navigate poorly written articles to get the core message of them.

With this in mind, I explored various text summarization techniques that would summarize articles that tickle my fancy.

## Code and Resources used
**Youtube tutorial:** https://www.youtube.com/watch?v=xvLQdP549NA

**Python Version:** 3.7

**Packages:** NLTK, Spacy, Flask, Gensim, sumy, BeautifulSoup

**Web App Requirements:** ```pip install -r requirements.txt```

## Summarizers
* **NLTK Summarizer** - 5 step Implementation.

    * Creating a word frequency table - create a dictionary for word frequency from the text without stopwords
    * Tokenization - splitting the text into a set of sentences
    * Scoring sentences - Using Term Frequency, we score a sentence by it's words, adding the frequency of every non-stop word in a sentence taking into account sentence length
    * Finding the threshold - setting the average score of the sentences as a threshold
    * Generate the summary -Only show sentences whose sentence score is more than the threshold

* **Spacy Summarizer** - Implementation is similar to NLTK