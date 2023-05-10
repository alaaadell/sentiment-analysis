# sentiment-analysis
A model to apply Sentiment Analysis of movie reviews using sentiment  polarity datasets (positive and negative)
## Introduction:
The project's main idea is to classify movie reviews to positive or negative. The objective
is to know a user or audience opinion on a target object by analyzing a vast amount of
text.
## Methodology:
### Data preprocessing:
Firstly, we appended all the reviews and their sentiments to a dataframe,
shuffled the rows, then we split the data to train(75%) and test(25%) sets
We remove any non alphabet character using regular expressions
We convert each word to lowercase
We remove the stop words
We apply lemmatization
We applied count vectorizer and TF IDF vectorizer and compared the
## results
### Models:
#### Random Forest classifier
With count vectorizer: 83% accuracy
With TF IDF vectorizer: 83.8% accuracy
#### Logistic Regression
With count vectorizer: 84.6% accuracy
With TF IDF vectorizer: 82% accuracy
#### Linear SVC
With TF IDF vectorizer: 84.8% accuracy (Best Model)
#### AdaBoost using decision tree classifier
With TF IDF vectorizer: 80.4% accuracy
### Conclusion: The best model with the highest accuracy is linear SVC used with TF IDF vectorizer (84.8% accuracy)
### Data Set Summary:
1. Data set used: polarity dataset v2.0
2. 1000 text files for positive reviews, and 1000 text files for negative
reviews, each file contains a paragraph about the movie either positive
or negative
a. note: We appended the reviews to a dataframe under a column
called review, and there’s a column called sentiment tells
whether the review is positive or negative
3. Data visualization:
#### Word cloud
![word cloud](https://user-images.githubusercontent.com/71910329/179066747-b7e568d6-c98e-48df-9e17-52b8d865d157.JPG)
 
### Visualizing results
![result](https://user-images.githubusercontent.com/71910329/179067258-450fded1-575b-4797-bf0a-262e546e6573.JPG)

