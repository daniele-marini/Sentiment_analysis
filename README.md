# Sentiment_analysis

## Problem 

The Sentiment analysis is a Natural Languages Processing task which, given an input text, return the "sentiment" of the given input.
It's a classification task that include 7 categories: Anger, Digust, Fear, Joy, Sadness, Surprise and Neutral.
The task is about creating a model that perform the classification given in input text/sentences

## Dataset

The dataset is composed of 58k texts labelled manually to assign them an emotion:
- Anger
- Digust
- Fear
- Joy
- Sadness
- Surprise
- Neutral

## Preprocessing

The preproceesing on the text/sentences include some operations that I considered necessary to make the dataset cleaner:
- edit in lower case
- remove emoji
- remove punctuation (except "?" and "!" )
- replace "?" with 'question' and "!" with 'esclamation'
- remove numbers
- remove stopwords

## Word embedding

For my model I decided to use a pre-trained embedded layer
I used an unsupervised learning algorithm for obtaining vector representations for words called GloVe
This dataset contains English word vectors pre-trained and there are from 25 up to 200 dimensional pre trained word vectors. I decided to use the 200 dimentional word vector

# Model

For the implementation of the neural nerwork I used 15 layers with a total number of about 6 milion of parameters
After several attempt with many different layer configurations I reached the best score (I took as a reference point the f1_score) using this configuration

# Results

After the evaluation of the model I reached as result a F1 Score equals to 0,59
