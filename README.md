# Kaggle-Spam
Spam Detection – Cluster SMS messages to “Spam” and “Ham” (Kaggle Challenge)

The SMS Spam Collection is a set of SMS tagged messages that have been collected for SMS Spam research. It contains one set of SMS messages in English of 5,574 messages, tagged acording being ham (legitimate) or spam.

I have Applied Random Forest algorithm validated using 5-fold GridSearchCV after feature creation to classify whether an incoming mail is a spam or not. Following techniques, packages and functions have been used:

* (Natural Language Toolkit) NLTK
* Tokenization
* Removal of Stopwords
* Stemming
* Lemmatizing
* Bag of Words (BoW) or CountVectorizer
* TF-IDF Vectorizer
* Feature Engineering
* Random Forest Classifier
* GridSearchCV
* Cross-Validation
* Model Evaluation metrics (precision, recall, fscore, accuracy, confusion matrix)

I have achieved an overall accuracy of 98% by implementing the Random Forest Algorithm on datasets modeled with both TF-IDF algorithm and Count Vectorizer method (Bag of Words) and compared their model evaluation metrics.

Using Random Forest algorithm for both TF-IDF Vectorizer model and Count Vectorizer model gave us the same values for all metrics:

TF-IDFVectorizer model: 
* Precision: 1.0 / Recall: 0.846 / F1-Score: 0.916 / Accuracy: 0.979
* Confusion Matrix for TF-IDFVectorizer model tells us that we correctly predicted 966 hams and 126 spams.0 hams were incorrectly identified as spams and 23 spams were incorrectly predicted as hams.

Count Vectorizer Model:
* Precision: 1.0 / Recall: 0.852 / F1-Score: 0.92 / Accuracy: 0.98
* Confusion Matrix for Count Vectorizer Model tells us that we correctly predicted 966 hams and 127 spams.0 hams were incorrectly identified as spams and 22 spams were incorrectly predicted as hams.

