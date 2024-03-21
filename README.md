# ArSen-20
Sentiment detection remains a pivotal task in natural language processing, yet its development in Arabic lags due to a scarcity of training materials compared to English. Addressing this gap, we present ArSen-20, a benchmark dataset tailored to propel Arabic sentiment detection forward. ArSen-20 comprises 20,000 professionally labeled tweets sourced from Twitter, focusing on the theme of COVID-19 and spanning the period from 2020 to 2023. Beyond tweet content, the dataset incorporates metadata associated with the user, enriching the contextual understanding. ArSen-20 offers a comprehensive resource to foster advancements in Arabic sentiment analysis and facilitate research in this critical domain.

The ArSen-20 dataset statistics:
| Statistics   |   Num  | 
|:-------------:|:-----:|
| Training set size | 16000 |
| Validation set size| 2000 |
| Testing set size | 2000 |
| Neutral | 17262 |
| Positive | 878 |
| Negative | 1860 |

## Features
The dataset has the following features:

⚠️ Please note that due to the restrictions imposed by [Twitter's Developer Agreement and Policy on Content redistribution](https://developer.twitter.com/en/developer-terms/agreement-and-policy), the data that we make public available does not comprise direct tweet text data and user privacy data.

| Field   |  Type  |  Description  |
|:-----------:| :--------: |:----------------: |
| tweet id     | string     | The unique identifier of the requested Tweet.     |
| label   | string     | Sentiment Classification of this tweet.     |
| author id   | string    |The unique identifier of this user.     |
| created_at  | data     | Creation time of the Tweet.    |
| lang  | string     | Language of the Tweet, if detected by Twitter.    |
| like_count  | int     |The number of likes on this tweet.|
|quote_count  | int    | The number of times this tweet has been quoted.    |
| reply_count   | int     | The number of replies to this tweet.    |
| retweet_count| int    | The number of retweets to this tweet.    |
| tweet❌   | string     | The actual UTF-8 text of the Tweet.    |
|user_verified  | boolean     | Indicates if this user is a verified Twitter User.     |
|followers_count  | int     |The number of followers of the author.     |
| following_count  | int     | The number of following of the author.    |
| tweet_count  | int     | Total number of tweets by the author.    |
| listed_count | int     |The number of public lists that this user is a member of.    |
|name❌ | string     | The name of the user.    |
| username❌   | string     | The Twitter screen name, handle, or alias.    |
| user_created_at| data     | The UTC datetime that the user account was created.     |
| description❌  | string     | The text of this user’s profile description (bio).     |

## DownLoad
You can download the dataset from [here](https://github.com/123fangyang/ArSen-20/tree/main/data).
+ ArSen-20_publish.csv - Contains all features except those marked with ❌ above.
+ ArSen-20_id_only.csv - Contains only tweets and their author's id.

You can get the source code of our request for tweet data to the Twitter API from here.
+ Twitter_API_Request.py - A Python script for accessing the Twitter API to collect data.
+ Data_Processing.py - A Python script for converting tweets json data to csv format.
+ Tweets_Preprocessing.py - A Python script for pre-processing tweets data.

## Citation
If you use this dataset in your research, please cite the following paper:

## contact
If you have any questions or comments about the dataset, please contact Yang Fang (20211209024@chnu.edu.cn).

Potential cooperation in related fields is also welcome. :)
