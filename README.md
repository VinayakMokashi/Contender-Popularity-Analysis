# BMC Election 2023 Winner Prediction Using Twitter Data (VADER + ML Algorithms)

This project aims to predict election outcomes by analyzing Twitter data from two political contenders, applying Machine Learning, VADER sentiment analysis, and popularity scoring. Using sentiment metrics and engagement data, it offers insights into public opinion and trends in popularity, ultimately predicting voter preferences and winner of the election.

## Project Overview:

This project leverages Twitter data to analyze and predict public sentiment toward two major political contenders, Contender A and Contender B, in an election scenario in Mumbai for BMC 2023 Elections. By combining sentiment analysis, popularity scoring, and engagement metrics, the study measures the impact of various tweet attributes on predicted election outcomes. Machine Learning and VADER sentiment analysis are key tools for understanding and interpreting public opinion.

## Data Collection and Description:

Tweets were collected using snscrape between June 30, 2022, and November 15, 2022, with approximately 50,000 tweets for each contender. Key data attributes include:

__Like Count__: Number of likes on each tweet.

__Retweet Count__: Number of retweets on each tweet.

__Username__: Twitter handle of the user posting the tweet.

__Date__: Date and time of each tweet.

__Tweet Content__: Text content of the tweet.

The raw datasets are processed to remove irrelevant characters, hashtags, links, and symbols, followed by language detection and filtering to include only English-language tweets.

## Methodology:

1. Data Preprocessing

__Text Cleaning__: Removed URLs, punctuation, extra spaces, and transformed text to lowercase.

__Stopword Removal__: Removed commonly used words (e.g., "the," "is," "and") that do not add significant meaning to the analysis, enhancing the focus on impactful words.

__Stemming and Lemmatization__: Standardized terms to their root forms, using techniques like stemming (e.g., "celebrating" to "celebr") and lemmatization (e.g., "celebrate" to "celebrate").

2. Sentiment Analysis (VADER)

Each tweet’s sentiment is calculated using the VADER sentiment scoring model, producing scores for positive, negative, and neutral sentiments.

Example sentiment scores: "A great leader" (0.6249), "A fine CM!" (0.2714), indicating varying degrees of public sentiment.

3. To capture meaningful features from text data, two vectorization methods were applied:

TF-IDF (Term Frequency-Inverse Document Frequency) Vectorization

Word2Vec Embeddings

4. Machine Learning Models

__Classification Models__: Several classification models (e.g., SVM, Naive Bayes) are applied to classify tweets as supportive, unsupportive, or Neutral of a contender based on sentiment.
Bagging and Boosting techniques and paramter tuning was done to obtain the best performing model.

5. Popularity Score:

A metric called as the popularity score was designed to predict the winner of the elections. The end results were accurate. 

## Key Findings:

__Popularity Trends__: Popularity scoring revealed a consistent trend, with one contender showing a higher popularity score, correlating with the positive sentiment in their tweets.


## Usage

Files Included:

__Raw Data__: Eknath_RawTweets.csv and Uddhav_RawTweets.csv containing tweet data (Contained in Raw_Tweets.zip)

__Scripts__:

Code.ipynb: End to end code implementatiom

Presentation.pdf: Project documentation and detailed explanations of methodologies and findings.

## Running the Analysis:

Install Requirements: Install necessary libraries like snscrape, nltk, vaderSentiment, sklearn, and wordcloud.

Execute Scripts: Run the script in sequence 

## Conclusion and Recommendations:

This analysis demonstrates that Twitter data can serve as a valuable predictor of public opinion, with sentiment analysis and popularity scores aligning closely with real-world election results. 

Recommendations include:

Focusing on tweet engagement strategies that drive positive sentiment.

Monitoring popularity scores for real-time insights into public opinion.

## Future Scope:

__Incorporating Additional Features__: Adding hashtag analysis, location data, and time-of-day effects to capture more nuanced sentiment patterns.

__Real-Time Prediction__: Extending the model for real-time tweet analysis to monitor changing trends and sentiment shifts as they happen.

__Deep Learning Models__: Applying advanced NLP techniques like BERT for improved sentiment classification accuracy.

