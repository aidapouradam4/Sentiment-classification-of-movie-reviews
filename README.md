# Sentiment-classification-of-movie-reviews
# Introduction
This project aims to present a binary classification model for sentiment analysis of reviews collected from the IMDB, Amazon, and Yelp websites. The dataset used for this project includes 3000 reviews, which were split into 2400 training and 600 testing datasets. Although the assumed audience of these websites is primarily English speakers, the data contains slang, misspellings, foreign characters, and other linguistic challenges that make natural language processing difficult. The primary objective of this project is to develop a binary classifier that can accurately identify the sentiment of a new sentence. This report will discuss the methods and techniques employed to develop this classifier and evaluate its performance on the test set.

# Methodology:

1. Bag-of-Words (BoW): BoW is used to convert text data into numerical form. It involves vocabulary creation, data cleaning, stemming, and feature extraction. The vocabulary size is around 2,858 words, and unigrams (single words) are used for feature representation.
2. Handling Out-of-Vocabulary Words: A method for handling out-of-vocabulary words in the test set is described, ensuring consistency with the training data.
3. Cross-Validation and Hyperparameter Selection: GridSearchCV is employed to tune hyperparameters using a three-fold cross-validation technique. The best hyperparameters are chosen for each model.
4. Analysis of Predictions: Examples of false positives and false negatives for the Naïve Bayes classifier are provided to analyze model performance.
5. Comparison of Model Performance: The report assesses whether the model performs better on longer or shorter sentences, as well as on reviews from different sources (Amazon or IMDB) and sentences with or without negation words.
6. Performance on Test Set: The performance of four classifiers (Logistic Regression, Naïve Bayes, Support Vector Machine, and Random Forest) on both the test and validation sets is summarized. Naïve Bayes achieved the highest accuracy.
   ![Screenshot 2023-10-02 183458](https://github.com/aidapouradam4/Sentiment-classification-of-movie-reviews/assets/103252922/7a96fcff-4d03-4562-9b08-d8dee6990e1a)

8. Testing the Model: The selected model is tested with two new sentences, which it correctly predicts.

# Outcome:

* The Naïve Bayes classifier achieved the highest accuracy on both test and validation sets.
  ![image](https://github.com/aidapouradam4/Sentiment-classification-of-movie-reviews/assets/103252922/2b7a8540-7340-42b6-95e8-c5bafabdaa41)

* The model generally performs slightly better on sentences with fewer words (less than 12).
* Among the sources, Amazon reviews had the highest percentage of correct predictions.
* The model performs better on sentences without negation words.
* The performance differences between the test and validation sets could be attributed to various factors, including data distribution, sampling variability, and overfitting.


