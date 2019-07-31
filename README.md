# Amazon-Fine-Food-Reviews-Sentimental-Analysis
- Amazon-Food-Reviews-Analysis-and-Modelling Using Various Machine Learning Models
- Performed Exploratory Data Analysis, Data Cleaning, Data Visualization and Text Featurization(BOW, tfidf, Word2Vec). Build several ML models like KNN, Naive Bayes, Logistic Regression, SVM, Random Forest, GBDT, LSTM(RNNs) etc.

### Objective:
  - Given a text review, determine the sentiment of the review whether its positive or negative.

#### Data Source: https://www.kaggle.com/snap/amazon-fine-food-reviews

#### About Dataset
The Amazon Fine Food Reviews dataset consists of reviews of fine foods from Amazon.


* Number of reviews: 568,454
* Number of users: 256,059
* Number of products: 74,258
* Timespan: Oct 1999 - Oct 2012
* Number of Attributes/Columns in data: 10


### Attribute Information:

* Id
* ProductId - unique identifier for the product
* UserId - unqiue identifier for the user
* ProfileName
* HelpfulnessNumerator - number of users who found the review helpful
* HelpfulnessDenominator - number of users who indicated whether they found the review helpful or not
* Score - rating between 1 and 5
* Time - timestamp for the review
* Summary - brief summary of the review
* Text - text of the review

#### Amazon Food Reviews EDA, NLP, Text Preprocessing and Visualization using TSNE
#### Defined Problem Statement
Performed Exploratory Data Analysis(EDA) on Amazon Fine Food Reviews Dataset plotted Word Clouds, Distplots, Histograms, etc.
Performed Data Cleaning & Data Preprocessing by removing unneccesary and duplicates rows and for text reviews removed html tags, punctuations, Stopwords and Stemmed the words using Porter Stemmer
Documented the concepts clearly
Plotted TSNE plots for Different Featurization of Data viz. BOW(uni-gram), tfidf, Avg-Word2Vec and tf-idf-Word2Vec

#### KNN
- Applied K-Nearest Neighbour on Different Featurization of Data viz. BOW(uni-gram), tfidf, Avg-Word2Vec and tf-idf-Word2Vec
- Used both brute & kd-tree implementation of KNN
- Evaluated the test data on various performance metrics like accuracy also plotted Confusion matrix using seaborne

#### Naive Bayes
- Applied Naive Bayes using Bernoulli NB and Multinomial NB on Different Featurization of Data viz. BOW(uni-gram), tfidf.
- Evaluated the test data on various performance metrics like accuracy, f1-score, precision, recall,etc. also plotted Confusion matrix using seaborne
- Printed Top 25 Important Features for both Negative and Positive Reviews

#### Logistic Regression
- Applied Logistic Regression on Different Featurization of Data viz. BOW(uni-gram), tfidf, Avg-Word2Vec and tf-idf-Word2Vec
- Used both Grid Search & Randomized Search Cross Validation
- Evaluated the test data on various performance metrics like accuracy, f1-score, precision, recall,etc. also plotted Confusion matrix using seaborne
- Showed How Sparsity increases as we increase lambda or decrease C when L1 Regularizer is used for each featurization
- Did pertubation test to check whether the features are multi-collinear or not

#### SVM
- Applied SVM with rbf(radial basis function) kernel on Different Featurization of Data viz. BOW(uni-gram), tfidf, Avg-Word2Vec and tf-idf-Word2Vec
- Used both Grid Search & Randomized Search Cross Validation
- Evaluated the test data on various performance metrics like accuracy, f1-score, precision, recall,etc. also plotted Confusion matrix using seaborne
- Evaluated SGDClassifier on the best resulting featurization

#### Decision Trees
- Applied Decision Trees on Different Featurization of Data viz. BOW(uni-gram), tfidf, Avg-Word2Vec and tf-idf-Word2Vec
- Used both Grid Search with random 30 points for getting the best max_depth
- Evaluated the test data on various performance metrics like accuracy, f1-score, precision, recall,etc. also plotted Confusion matrix using seaborne

#### Ensembles(RF&GBDT)
- Applied Random Forest on Different Featurization of Data viz. BOW(uni-gram), tfidf, Avg-Word2Vec and tf-idf-Word2Vec
- Used both Grid Search with random 30 points for getting the best max_depth, learning rate and n_estimators.
- Evaluated the test data on various performance metrics like accuracy, f1-score, precision, recall,etc. also plotted Confusion matrix using seaborne
- Plotted world cloud of feature importance recieved from the RF and GBDT classifier

#### LSTM(RNNs)
- Applied different architectures of LSTM on Amazon fine food reviews dataset
- Recurrent Neural Networks(RNN) with one LSTM layer.
- Recurrent Neural Networks(RNN) with two LSTM layer.

