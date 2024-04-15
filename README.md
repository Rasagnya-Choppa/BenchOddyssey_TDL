# TOPICS WITH DEEP LEARNING

   TEAM : BENCH ODYSSEY
   TEAM NO: 23
   
- PES2UG21CS148 Choppa Rasagnya
- PES2UG21CS158 Deepika Indran
- PES2UG21CS160 Devansh Guttikonda

## Predicting the Likes Count of a YouTube Video

A command line tool to model the likes count of a YouTube video as a function of various
features. Since this task focused on feature engineering I have tried to obtain relevant features for the data set from different
methods and sources. I have used the YouTube API to gather video details such as -
- Video_id
- Title
- PublishedAt
- ChannelId
- ChannelTitle
- Trending_Date
- Tags
- View Count
- Likes
- Comment Count
- Thumbnail_Link etc

The following features was used to predict the likes
- view_count
- comment_count
- Sentiment_Scores
- time_till_trend
- Subscriber_Count

The model which we used was the XGBoost (Extreme Gradient Boosting). XGBoost is an ensemble learning technique that combines multiple decision trees to improve predictive performance.
- R-square: 0.9597375701889096
- RMSE:110538.93938925382
- MAE:31216.7363869918

## How to Use

1) <code>git clone TDL_PROJECT_CODE_Team23.ipynb</code>

2) <code>cd YouTube-Video-Like-Count-Predictor</code>

3) Run the <code>test_input.py</code> and provide the video ID as system arguement.

## Limitations
Over time the predictions have to be run again as its not real time.

## Conclusion and Future Work
Market Analysis:
Analyze trends in video popularity, viewership, and engagement to understand audience preferences and behavior in the Indian market.

Thumbnail Analysis:
Identify the influence of a thumbnail of a video and how it performs using CNN’s and other Deep learning techniques. 

Sentiment Analysis: 
Utilize comments data to gauge audience sentiment towards specific topics or creators, aiding in reputation management and content optimization strategies.

