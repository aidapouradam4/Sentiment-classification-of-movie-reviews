# Sentiment-classification-of-movie-reviews
# Introduction
This report aims to present a binary classification model for sentiment analysis of reviews collected from the IMDB, Amazon, and Yelp websites. The dataset used for this project includes 3000 reviews, which were split into 2400 training and 600 testing datasets. Although the assumed audience of these websites is primarily English speakers, the data contains slang, misspellings, foreign characters, and other linguistic challenges that make natural language processing difficult. The primary objective of this project is to develop a binary classifier that can accurately identify the sentiment of a new sentence. This report will discuss the methods and techniques employed to develop this classifier and evaluate its performance on the test set.

# Methodology:

1. Bag-of-Words (BoW): BoW is used to convert text data into numerical form. It involves vocabulary creation, data cleaning, stemming, and feature extraction. The vocabulary size is around 2,858 words, and unigrams (single words) are used for feature representation.
2. Handling Out-of-Vocabulary Words: A method for handling out-of-vocabulary words in the test set is described, ensuring consistency with the training data.
3. Cross-Validation and Hyperparameter Selection: GridSearchCV is employed to tune hyperparameters using a three-fold cross-validation technique. The best hyperparameters are chosen for each model.
4. Analysis of Predictions: Examples of false positives and false negatives for the Naïve Bayes classifier are provided to analyze model performance.
5. Comparison of Model Performance: The report assesses whether the model performs better on longer or shorter sentences, as well as on reviews from different sources (Amazon or IMDB) and sentences with or without negation words.
6. Performance on Test Set: The performance of four classifiers (Logistic Regression, Naïve Bayes, Support Vector Machine, and Random Forest) on both the test and validation sets is summarized. Naïve Bayes achieved the highest accuracy.
7. Testing the Model: The selected model is tested with two new sentences, which it correctly predicts.

# Outcome:

* The Naïve Bayes classifier achieved the highest accuracy on both test and validation sets.
* The model generally performs slightly better on sentences with fewer words (less than 12).
* Among the sources, Amazon reviews had the highest percentage of correct predictions.
* The model performs better on sentences without negation words.
* The performance differences between the test and validation sets could be attributed to various factors, including data distribution, sampling variability, and overfitting.

In summary, the report presents the development and evaluation of a sentiment analysis model using various techniques and analysis of its performance on different aspects, ultimately highlighting the strengths and weaknesses of the approach.
