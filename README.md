# vaccine-tweet-sentiment-analysis
This project is a sentiment analysis project using the Twitter API, tweepy library, and a Naive Bayes Classifier to investigate public sentiment toward the COVID-19 Vaccine.

# Process
For this project, I used the Twitter API and the tweepy library to create a dataframe of recent tweets with the keyword (#covidvaccine). This data was unprocessed, so I cleaned up the tweets, and added more data by gathering the polarity, subjectivity, and analysis of each tweet. This information can be viewed in the csv file included called 'covidtweets.csv'.

Afterwards, I created a few visualizations to quickly examine the overall trends in the tweets, which can be seen below.

I then used a trained a Naive Bayes Classifier to determine the sentiment of a given tweet, which came out to around 80% accuracy.  
