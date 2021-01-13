# vaccine-tweet-sentiment-analysis
This project is a sentiment analysis project using the Twitter API, tweepy library, and a Naive Bayes Classifier to investigate public sentiment toward the COVID-19 Vaccine.

# Process
- gather and clean data
- visualize tweet data
- train classifier (Naive Bayes)
- test classifier

For this project, I used the Twitter API and the tweepy library to create a dataframe of recent tweets with the keyword (#covidvaccine). This data was unprocessed, so I cleaned up the tweets, and added more data by gathering the polarity, subjectivity, and analysis of each tweet. This information can be viewed in the csv file included called 'covidtweets.csv'.

# Visualizations
Afterwards, I created a few visualizations to quickly examine the overall trends in the tweets, which can be seen below. I explained in my Jupyter Notebook, but a few observations include: 

![Word Cloud of Tweets](https://github.com/kickflipped/vaccine-tweet-sentiment-analysis/blob/main/Figures/wordcloud.png)

* many of the popular words in these tweets are generally neutral or positive, not many explicitly negative words that appear repeatedly
* words such as "second dose", "first dose", "distribution", "rollout", and "school" show up, which may indicate that these are some of the popular topics of discourse regarding the vaccine (e.x. people are discussing their experiences with getting various dosages, the methods in which the vaccine is being distributed, how this might impact structures such as schools)

![Scatterplot of Tweet Sentiment](https://github.com/kickflipped/vaccine-tweet-sentiment-analysis/blob/main/Figures/scatter.png)

* more tweets fall in the neutral or positive end of the spectrum than the negative end. Discourse on the COVID Vaccine is largely supportive (shown below as well)
* the spread of subjectivity is also very wide, but it seems that few of the tweets are entirely subjective

![Bar Graph of Tweet Sentiment](https://github.com/kickflipped/vaccine-tweet-sentiment-analysis/blob/main/Figures/bar.png)

# Training and Testing
I then used a trained a Naive Bayes Classifier to determine the sentiment of a given tweet, which came out to around 80% accuracy (see code). I randomly gathered 9 tweets under the same classifier to test my model, and found that generally, the model was very good at classifying positive tweets correctly, but sometimes had trouble evaluating neutral tweets, which indicates some false positives and false negatives, due to evaluating neutral tweets (e.x. just informative tweets) as pos/neg.

# Notes for Improvement in the Future
In the future, I want to retrain my model using a larger data set. The covid vaccine is a highly debated topic across the internet, and would benefit from a larger set of tweets to improve sentiment analysis. I would also want to grab tweets for testing my model in the same
manner that I did to obtain the tweets for training. This would also give me a better test for how my classifier is doing.

# Conclusions
This Sentiment Analysis was very helpful in determining the overall sentiments that people are having about the vaccine, which leans positive. It was also really interesting to use my visualizations to see what types of subtopics about the vaccine are being widely discussed (such as distribution and schools). This could open doors for more data analysis about these specific topics, and hep determine what people are thinking about these specific discussions.
