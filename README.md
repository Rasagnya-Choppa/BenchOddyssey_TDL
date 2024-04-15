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
- View Count
- Comment Count
- Dislike Count
- Favorite Count
- Life of video
- Duration
- Category etc.

Another set of features was gathered from the characteristics of the channel via which the video was uploaded. Some of the features in this category were -
- Channel Subscriber Count
- Channel View Count 
- Channel Video Count
- Channel Comment Count

The third method I used for feature engineering was finding out the number of times the video was shared on other social media platforms such as Facebook, Google Plus, Linkedin and Pinterest. Hence the next 5 features were generated as well -
- Facebook Shares
- Google Plus Shares
- LinkedIn Shares
- Pinterest Shares
- Total Shares

The model which we used was the XGBoost (Extreme Gradient Boosting). XGBoost is an ensemble learning technique that combines multiple decision trees to improve predictive performance.
- R-square=0.95
- MSME
- MSE

## How to Use
I have developed a command line tool to test out the model. 

1) <code>git clone https://github.com/mayank26saxena/YouTube-Video-Like-Count-Predictor.git</code>

2) <code>cd YouTube-Video-Like-Count-Predictor</code>

3) Run the <code>test_input.py</code> and provide the video ID as system arguement.

## Limitations
The file <code>get_data.py</code> can be run by providing the video ID as a command line arguement. The output will be the predicted like count , the actual like count and the error.

The high error in a few cases can be attributed to the fact that the data set is highly skewed with large number of videos having single digit or no likes but very few videos having likes greater than 10,000 with the highest like count of any video in the data set being <code>936889</code>

This error can be improved by collecting more data so that the data set is less skewed and more evenly distributed.

## Conclusion and Future Work
Market Analysis:
Analyze trends in video popularity, viewership, and engagement to understand audience preferences and behavior in the Indian market.

Thumbnail Analysis:
Identify the influence of a thumbnail of a video and how it performs using CNN’s and other Deep learning techniques. 

Sentiment Analysis: 
Utilize comments data to gauge audience sentiment towards specific topics or creators, aiding in reputation management and content optimization strategies.

