# Sentiment Classification of Nuclear Energy Tweets

Through classification modeling, this project aims to classify the sentiment of tweets on nuclear energy as positive, negative or neutral.

As the necessity for alternative energy resources increases due to climate change, the discussion around nuclear energy is impossible to avoid as it is a key contender. However, nuclear energy has become a divisive and polarizing topic - and so, we wanted to understand if sentiment could be easily identified around nuclear energy and what that looks like.

Predicting the sentiment of a certain tweet around nuclear energy, allows companies and lawmakers to identify specific words or phrases around nuclear energy that lend to a negative or positive perception. This allows messaging to be tailored to a specific audience without being oblivious to their opinions. For example:

  - Focusing on solutions connected to the negative words can help address concerns.
  - Highlighting the positive words can amplify the support of nuclear energy.


## Data:

Our dataset contained 3,000 tweets scraped via Twint from Twitter using the search term 'Nuclear Energy'. All tweets were pulled from 2020. The sentiment of each tweet was trained using Vader and modification of its metrics. The three sentiments used in this project were: Positive, Negative and Neutral.

![](/images/target.png)

## EDA - Word Frequencies:

Our inital EDA focused on visualizing word frequency for each sentiment class and analyzing the most frequent words of each. Clear differences in vocabulary was observed: 
Positive - Clean, Support, Need
Negative - Waste, Danger
Neutral - Research/ informational topics such as different types of renewable energy.

We also were able to analyze that the sentiment distribution in our dataset was unbalanced - most tweets fell under 'neutral' followed by positive and then negative.  This would need to be accounted for in our modeling. 

![](/images/pos.png)
![](/images/neg.png)
![](/images/neu.png)


## Conclusion:

The use of social media such as Twitter has been such an important tool for capturing public opinion on any and all topics. This is vital information for companies and policymakers alike. Classifying the sentiment of tweets around nuclear energy shines a light on specific issues and themes regarding this topic. Using SVM we were able to predict sentiment with over 82% accuracy and therefore, extract key words and themes as they relate to each sentiment. These insights can be really useful for marketing and PR strategies, whether its for an election or pitching a nuclear energy project.

For example, the top negative word from our analysis is "waste", which concludes that the public's concern is greatly around nuclear waste and its consequences rather than the energy source itself. Companies/Lawmakers can then reassure the public that this is also their main concern regarding nuclear and that may help change negative opinions.

One of the top positive words is safe, which companies can then emphasize when promoting nuclear energy.




![](/images/svmpos.png)
![](/images/svmneg.png)
![](/images/svmneu.png)


## Contents of this repository: 

1. Data folder - all relevant csv files 
2. Working Notebook folder - twint script, cleaning & eda, modeling 
3. Final.ipynb - final notebook 
4. Nuclear Tweets.pdf - presentation deck
