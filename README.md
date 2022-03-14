# What Sentiment Analysis Can Reveal About Common Speech Patterns

## Digital Humanities 140 Coding for Humanities with Professor Winjum at UCLA Winter 2022

#### 3/14/2022 | Crystal Huynh, Larry Qu, Nelson Truong

### Introduction

#### Project Overview
This project analyzes the sentiment of a movie reviews dataset using Python through Jupyter Notebooks. 

#### Research Question: What common speech patterns can be found in positive and negative commentary?
Our group wanted to explore how people tend to speak when talking in an extremely positive and negative manner, especially in the context of movie reviews. Are there specific words that are frequently used when speaking in a positive sentiment versus a negative one? How often do those words show up in speech? How polarizing are these frequently used words? Do people tend to speak more when they are feeling positive or negative about something? This is the first step that we want to take when analyzing the speech patterns of movie reviews.

#### Why It Matters
With this information, we can later see whether these patterns match typical human behavior/speech, or if they are more specific in an online, more anonymous environment. We can use our findings to potentially see how polarizing these spaces are and how they affect our society in the long run as this type of analysis can also be used on things like social media comments and news articles where commentary can be even more polarizing. As we explore speech patterns in settings outside of normal, in person conversation, we can get a better idea of how people truly think and feel in certain environments or how people will think and feel given what we already know. 

### Methods

#### Data Source
[IMDB Dataset of 50K Movie Reviews](https://www.kaggle.com/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)

[More Dataset Information](http://ai.stanford.edu/~amaas/data/sentiment/)

We are using the IMDB Dataset of 50K Movie Reviews Large Movie Review Dataset from kaggle which contains 50K movie reviews. This dataset can be used for binary sentiment classification as it contains highly polar positive and negative movie reviews for training and testing.

The dataset contains two columns, one which contains the movie review text and the other with its corresponding sentiment categorization of positive or negative. Both the review and sentiment columns are object data types which represent strings.

We also need to acknowledge the shortcomings of our dataset. Although there is not much information on where the reviews are from, we can assume the reviews cover multiple movies. With that being said, we also do not know what time period these reviews are from, the criteria for being described as "highly polar", or the backgrounds of the people who made these reviews. The context in which these reviews were made would have provided more insight into common behavioral patterns.  

[Negative Words](https://gist.github.com/mkulakowski2/4289441)

[Positive Words](https://gist.github.com/mkulakowski2/4289437)

In order to identify the positive and negative words, we can easily scan the web for premade datasets. These two shown above are datasets containing negative and positive words, respectively, that we can use to analyze our movie reviews with. These datasets may help us recognize whether a review is actually negative/positive based on the words used, the most common words used in a negative/positive statement, how the context matters when using negative/positive words, and other speech patterns.

#### Project Scope
The intended analysis is to see what are the common "positive" and "negative" words being used and how often they are used. The resulting visualizations for this would probably be something like a bar chart highlighting the ten most common "positive" and "negative" words and how often they appear in the dataset. We can also how long "positive" reviews are compared to "negative" reviews by checking the word count for each review and plotting the total word count frequency in a separate bar chart. Another analysis we could do is categorize common "positive" and "negative" words to see how polarizing they really are and plot this on another bar chart to visualize the scale of how positive "positive" reviews are and how negative "negative" reviews are.

#### Analytical Process
We will first start by exploring our dataset as a whole to better understand how we can utilize the data we have to answer our research question. We know that the dataset contains both positive and negative reviews, so we will also explore the positive and negative reviews separately. We'll conduct a word frequency analysis to see what kinds of words are being used in a negative/positive context. Within our word frequency analysis, we'll also take a look at the sentiment of each word to understand the vocabulary being used and how they may affect the overall review. When looking at positive and negative reviews as a whole, we'll calculate a sentiment score on each review to compare the score with the original sentiment categorization to understand the accuracy of our analysis. We'll also calculate the average positive and negative review sentiment scores and compare them with each other. Lastly, we'll look into how the length of the reviews affect the strength of the review's sentiment.
