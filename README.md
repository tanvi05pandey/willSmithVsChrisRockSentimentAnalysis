# willSmithVsChrisRockSentimentAnalysis
An analysis of Tweets on the famous slap of Oscar 2022

## Data Collection:
The data has been scraped off of Twitter using **snscrape** - a scraper for social networking services (SNS). The tweets are dated from March 27, 2022 00:00:00 hours to March 28, 2022 23:59:59. I scraped the tweets seperately for Will Smith and Chris Rock in a file called twitterDataOscar.csv and twitterDataOscarChris.csv, respectively.

<img width="317" alt="image" src="https://user-images.githubusercontent.com/4620848/187547058-e8015052-a2ee-42c5-a484-402a410cd178.png">
<img width="1069" alt="image" src="https://user-images.githubusercontent.com/4620848/187549180-55927339-bb99-42bd-b535-e614654a78f1.png">
<img width="1065" alt="image" src="https://user-images.githubusercontent.com/4620848/187549271-9b4f9ebb-5f13-4d64-92ad-6ee15f141d23.png">


## Sentiment Analysis:
I import the NLTK library, along with the SentimentIntensityAnalyzer (SID) module. The SID module takes in a string and returns a score in each of these four categories - positive, negative, neutral, and compound. Before analyzing the sentiment of the tweets, I clean them using the function *clean* and create a new column called *tweet_clean*. After that, I calculate the compound polarity scores of cleaned tweets and save them in another column called *sentiment*. Now, I convert the compound scores into categories - 'positive', 'negative', and 'neutral' and save them in a new column called *sentiment_category*

## Visualization
Now that we have Tweets classified as positive and negative, let's take a look at changes in sentiment over time. Note that the red line denoted negative sentiment and green denotes positive.

**Overall Sentiment for Will Smith**
<img width="923" alt="image" src="https://user-images.githubusercontent.com/4620848/187550130-60c5997e-4799-4806-8e04-1607160904a2.png">

**Overall Sentiment for Chris Rock**
<img width="915" alt="image" src="https://user-images.githubusercontent.com/4620848/187550359-55d62a28-76cb-4717-9c03-43230dad33ca.png">

**Observation:**
Clearly the total number of tweets mentioning Will Smith are far greater than Chris Rock. However, when it comes to positive and negative emotions, the difference between positive and negative sentiments for Will Smith isn't much, while it is much greater for Chris Rock. The overall feeling is positive for both the actors.

**Most prominent positive words for Will Smith**

<img width="448" alt="image" src="https://user-images.githubusercontent.com/4620848/187551430-5601f041-bef0-4cc6-b44f-8465002987eb.png">

**Most prominent positive words for Chris Rock**

<img width="405" alt="image" src="https://user-images.githubusercontent.com/4620848/187551483-460579cb-6ab0-48c1-9b8f-424cf62dd3f8.png">

**Most prominent negative words for Will Smith**

<img width="363" alt="image" src="https://user-images.githubusercontent.com/4620848/187551612-2c648ecb-7482-45cb-9e6c-b42f4e3f79b7.png">

**Most prominent negative words for Chris Rock**

<img width="363" alt="image" src="https://user-images.githubusercontent.com/4620848/187551654-3edfeabf-353b-4fa1-b22a-8bd45dc830ad.png">

That's all for this analysis!

