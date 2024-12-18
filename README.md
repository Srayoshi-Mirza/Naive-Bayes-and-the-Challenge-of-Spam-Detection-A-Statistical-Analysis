
# Naive Bayes and the Challenge of Spam Detection A Statistical Analysis

## Overview

This project explores the application of the Naive Bayes algorithm to classify emails as "spam" or "not spam" using a simple Excel-based approach. The project highlights the core principles of Naive Bayes, including prior and conditional probabilities, and explores the limitations of the "naive" independence assumption, particularly in the context of spam email classification.

## Acknowledgements

 - [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
 - [Awesome README](https://github.com/matiassingers/awesome-readme)
 - [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)


## Objectives

- Demonstrate the application of Naive Bayes in a simple, practical scenario using Excel.
- Calculate the posterior probabilities of new emails being spam or not based on keyword occurrences and prior probabilities.
- Recognize the key assumption in Naive Bayes: that features are conditionally independent given the class.
- Observe the limitations of the "naive" assumption and its effect on prediction accuracy.
- Classify a set of emails as "spam" or "not spam" and evaluate the Naive Bayes classifier's accuracy.
- Analyze the impact of zero-frequency features on model performance.
- Critically assess the effectiveness of Naive Bayes for spam email classification based on the dataset provided.

## Datasets

### Training Data

- Dataset: [Spam Email Dataset](https://www.kaggle.com/datasets/jackksoncsie/spam-email-dataset)
- Description: This dataset contains a collection of email messages, labeled as either "spam" or "not spam". It serves as the training data to build and evaluate the Naive Bayes classifier.

### Testing Data

- Dataset: [Email Spam Dataset](https://www.kaggle.com/datasets/nitishabharathi/email-spam-dataset)
- Description: This dataset includes another collection of email messages, which will be used to evaluate the performance of the trained Naive Bayes classifier.

## Methodology

1. Data Preprocessing:

- Extracted key features such as keywords ("Offer" and "Win") from the email text.
- Calculated prior probabilities (P(Spam) and P(Not Spam)) based on the training data.

![Train Data](https://github.com/Srayoshi-Mirza/Naive-Bayes-and-the-Challenge-of-Spam-Detection-A-Statistical-Analysis/blob/6b4997ee01a054ae83248ccf5b06d7cdce71bc58/Images/train.jpg)

![Test](https://github.com/Srayoshi-Mirza/Naive-Bayes-and-the-Challenge-of-Spam-Detection-A-Statistical-Analysis/blob/6b4997ee01a054ae83248ccf5b06d7cdce71bc58/Images/test%20data.jpg)
2. Conditional Probability Calculation:

- Calculated the conditional probabilities for the presence of the keywords given the email class (spam or not spam).
3. Posterior Probability Calculation:

- Using Bayes' Theorem, computed the posterior probabilities for each new email based on the keyword occurrences and prior probabilities.

![Calculation](https://github.com/Srayoshi-Mirza/Naive-Bayes-and-the-Challenge-of-Spam-Detection-A-Statistical-Analysis/blob/6b4997ee01a054ae83248ccf5b06d7cdce71bc58/Images/probability%20calculation.jpg)

## Methodology
4. Classification:

- Classified the test emails as either "spam" or "not spam" based on the calculated posterior probabilities. If P(Spam | Keywords) > P(Not Spam | Keywords), the email was classified as spam.
5. Evaluation:

- Evaluated the model's performance based on accuracy, precision, and recall.
- Analyzed the impact of zero-frequency features and the limitations of the Naive Bayes algorithm in this context.
## Results

Accuracy: 83%
Precision: 0
Recall: 0

The model performed poorly in classifying spam emails, demonstrating the challenges of using Naive Bayes in scenarios with correlated features and zero-frequency issues.

![Model Evaluation](https://github.com/Srayoshi-Mirza/Naive-Bayes-and-the-Challenge-of-Spam-Detection-A-Statistical-Analysis/blob/main/Images/model%20evaluation.jpg)

