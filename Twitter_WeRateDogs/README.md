# Twitter WeRateDogs Analysis
## Elemide Sofiyah


# Table of contents
1. [Introduction](#introduction)
    1. [Description](#description)
    

2. [References](#references)

## 1. Introduction <a name="introduction"></a>
The dataset that is wrangled, analyzed and visualized for this project  is the tweet archive of Twitter user @dog_rates with username WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs and adds a lighthearted comment.
I have collected the data related to the **WeRateDogs** in a number of formats and from sources using Python and its libraries, evaluated its quality, and then cleaned it.

### 1.1. Description <a name="description"></a>
The three different datasets that are required to complete this project is gathered by using twitter API. The datasets are described below:
1. **Enhanced Twitter Archive**
This dataset gathered and provided by Udacity contains basic tweet data for 2356 of WeRateDogs tweets. This dataset was downloaded directly from resources provided by Udacity and loaded into a dataframe with read_csv(). The dataset contains 17 columns, some of which are:
- **tweet_id** : the unique identifier of a tweet.
- **source** : where the tweet was uploaded
- **timestamp** : the exact date and time the tweet was uploaded
- **text** : comments in the tweet
- **ratings** : dog rating coined from text
- **name** : name of dog in the tweet

2. **Additional Data through the Twitter API**
This dataset contains the number of tweet like and number of retweet of each tweet, since each tweet has a unique tweet id. This data should be scraped from the twitter API(tweepy), however for some reason, I have not been granted access to use the API. Udacity provided a url for this file that should have been gathered from tweepy. Using Python's **requests** library, I was able to get the content of the url loaded to a file and read the content into a dataframe. The dataset has 3 columns:
- **tweet_id** : the unique identifier of a tweet.
- **retweet_count** : number of retweet the post or tweet got
- **favorite_count** : number of likes the tweet got

3. **Image Predictions File**
The url for this file was provided by Udacity, I just needed to get the content of the file using the **requests** library. An instructor ran each and every image in the WeRateDogs Twitter archive through a neural network that can classify breeds of dogs to get these additional columns: 
- **tweet_id** : the unique identifier of a tweet.
- **img_num** : number of images posted along with the comment, maximum is 4
- **p1** : neural network's first prediction for the image in the tweet
- **p1_conf** : how confident the algorithm is in its first prediction
- **p1_dog** : is the first prediction a breed of dog
- **p2** : neural network's second prediction for the image in the tweet
- **p2_conf** : how confident the algorithm is in its second prediction
- **p2_dog** : is the first prediction a breed of dog
- **p3** : neural network's third prediction for the image in the tweet
- **p3_conf** : how confident the algorithm is in its third prediction
- **p3_dog** : is the first prediction a breed of dog
   

## 2. References <a name="references"></a>
- [1]  WeRateDogs Profile on Twitter
https://twitter.com/dog_rates

- [2] Create a Twitter Developer's Profile
https://developer.twitter.com/en

- [3] Collect Data from Twitter API
-https://towardsdatascience.com/collect-data-from-twitter-a-step-by-step-implementation-using-tweepy-7526fff2cb31 

- [4] How to Choose a Chart Type
https://towardsdatascience.com/data-visualization-101-how-to-choose-a-chart-type-9b8830e558d6
