# A_A_winereviews
An analysis of 130 wine reviews using Naive Bayes classifier and Vader Sentiment Analysis

Hi! Thank you for checking out my analysis of wine reviews from Wine Enthusiast Magazine (courtesy of Zack Thoutt's 2017 scrape of winemag.com).

Each jupyter notebook has the results printed to the screen. Just open up a notebook to see the results.

If you are interested in running your own analysis you can find the altered and changed dataset files here: https://www.dropbox.com/sh/ybjsdpid0ym58lh/AACN30AtbpSeq9atIxlIvfMna?dl=0

1) Wine_Processing_SentimentAnalysis (f).ipynb contains my Text Blob Sentiment Analysis. I also performed a VADER sentiment analysis but visualized the results using tableau. If you would like the VADER analysis, please drop me an email.

2) Wine_Processing_SentimentAnalysis (f).ipynb contains my Naive Bayes classifier for the wine variety, "Pinot Noir". I was hoping to be able to classify the top 3 most reviewed wines, as each of them have around ~10k total reviews, but was limited by time.

## Feedback

Nice work, this is **complete**. 

Some other thoughts: 

* The adjective extractor is cool. It seems odd to me to store it as a list within a cell of the df. 
* The NB would be much better if we could see the most predictive features. 
* I'm curious what's in the `counts` object.
* It's odd to mix upper and lowercase: `X_train, X_test, y_train, y_test`
* That confusion heatmap would be nicer without having to do the exponentials in my head.
* You've already got `spacy`, why use `TextBlob`?
* You do a _lot_ of just printing DFs to the screen (or their heads). That's absolutely the
  bare minimum in terms of "analysis". I would have liked to see you do a more thorough job
  on the actual analysis. For instance, I'd like to see a scatterplot of points and sentiment. Similarly,
  more on the group by variety, but only for the top variatals. I know that just putting the 
  stuff together was the real challenge here, though. 
* Is the first word cloud all wines? You never really say that I can see. It'd be nice to just use some 
  headers to orient me.
* Wordclouds are super cool. You should sell those on Zazzle glasses. 
* Sentiment notebook ends pretty abruptly. 
