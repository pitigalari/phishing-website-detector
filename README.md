**Decision Tree based**
# Phishing Website Detector

Phishing websites are websites created to be very similar to the genuine websites of credible companies. Since these are equivalent to the legitimate ones, users are easily defrauded by them. Phishing attacks usually start with an email that asks users to update or validate their information by visiting the link given. When users click on such links they are redirected to phishing websites where they are asked to enter sensitive personal information such as usernames, passwords or credit card and bank account information. This helps attackers to carry out financial frauds eventually with the stolen information. With the number of phishing websites on the rise, it has become a serious problem even for experienced users to protect their valuable information from fraudulent persons.

The basic idea of creating a phishing detector is to train a model to identify a special set of characteristics of websites by the URL of that particular site.

<a href="https://colab.research.google.com/github/roshsoftco/phishing-website-detector/blob/1.1/model.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

## Dataset

The dataset was obtained from the UCI Machine Learning Repository. It is a complete numerical dataset with over 11,000 instances.
First, the data set was separated into 3 categories as the training set, validation set and testing set as 75%, 20% and 5% (approx.) respectively and saved into separate CSV files.

Use the following link to download the dataset,
https://archive.ics.uci.edu/ml/datasets/Phishing+Websites

## Architecture

The developed AI-based software application uses the Decision Tree model to predict phishing websites using 30 different features in the URL.
The features can be mainly categorise into,
 * URL Bar Features
 * Irregular Features
 * HTML & JS Features
 * Domain Features
 
 SciKit-Learn’s DecisionTreeClassifier is used as the model along with Entropy as the splitting criterion.
 
 ## Performance
 
 The trained model maintains a mean accuracy level of 89% as a percentage. The accuracy was measured using the `score(x, y)` function in the DecisionTreeClassifier.
