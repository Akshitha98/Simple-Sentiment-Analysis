# Simple-Sentiment-Analysis

VADER is an NLTK module that provides sentiment scores based on words used ("completely" boosts a score, while "slightly" reduces it), on capitalization & punctuation ("GREAT!!!" is stronger than "great."), and negations (words like "isn't" and "doesn't" affect the outcome).

VADER's SentimentIntensityAnalyzer() takes in a string and returns a dictionary of scores in each of four categories:
* negative
* neutral
* positive
* compound (computed by normalizing the scores above)

We apply SentimentIntensityAnalyzer to a dataset. The dataset used here is amazom reviews. These are labeled as either "pos" or "neg". At the end we'll determine the accuracy of our sentiment analysis with VADER. 

**Accuracy is given by the formula:   
 (True Positive+True Negative)/Total**                   
where True Positive is the number of positive predictions which are labeled as positive.
                              True Negative is the number of negative predictions which are labeled as negative.
                              Total is the total number of predictions.
      
And finally we use scikit-learn to determine how close VADER came close to original labels. This is obtained by confusion martix.
Confusion matrix is the organised representation of predicted values compared to the real values.
