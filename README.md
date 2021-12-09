# Document-Classification-Algorithm
This repository contains project resources to create a document classification algorithm in practise

Title: **Document Classification using Hierarchical Attention Networks**

Author: 
* Vinayak Sengupta (vs4016@rit.edu)


About:

The goal of the project is to support software developers in improving the quality of their code by the recommendation of the appropriate refactoring strategies to address Self-Admitted Technical Debt (SATD). To do so, we are designing and implementing a recommendation model that takes as input of existing SATD comments, and recommends the appropriate refactoring operations that needs to be performed as part of addressing the debt in the comment. Along with that we are also going to be classifying among which SATD comments is refactoring even required.


## Requirements

* Python 3 (3.8+)
* json
* numpy (1.18.5)
* pandas (1.0.5)
* Matplotlib (2.2.4)
* Pydot
* scikit-learn
* spacy
* tensorflow==2.3.0
* tqdm
* scikit-learn (0.23.1)
* natural language tool kit (3.5)
* keras (2.4.0)

## Dataset

An analysis of 50,000 IMDB movie reviews was conducted for the labeled data set. Reviews are scored as binary sentiment, so a 5-star IMDB rating results in a score of 0, and a rating >=7 results in a score of 1. The sentiment of reviews is derived from what is written about each movie. It does not contain any movies that are part of the test set with 25,000 reviews. Furthermore, IMDB reviews without labels are available for another 50,000 titles.
.  

* The frequency of number sentences in the document

![image](https://user-images.githubusercontent.com/34100245/145473234-861ccc74-cb1f-479d-b3a9-435efe678ad9.png)


## Models used
* Random Forest Classifier
* Logistic Regression
* Support Vector Machine (SVM)
* Multi Nomial Naive Bayes (MNB)
* Convolutional neural network (CNN)
* Long short-term memory (LSTM)

## Result
|Model | F1 score | +MLSMOTE | Accuracy |  +MLSMOTE | Time|
|--- | --- | --- | --- |--- |--- |
|RF | 0.73 | 0.68 |0.46| 0.36 | 1.5 min | 
|LR | 0.71 | 0.67 |0.40  | 0.30 | 9.21 min| 
|SVM | 0.66  | 0.65 |0.32 | 0.33 | 8.92 min |
|MNB | 0.67  | 0.66  |0.35 | 0.29 | 1.2 min|
|MLP | 0.73 | 0.69 |0.46 | 0.34 | 33 min |
|CNN | 0.62 |  0.61 |0.73 | 0.70 | 7.33 min|
|LSTM | 0.61 | 0.60 |0.71| 0.71 |42 min|


## How to Run
* Clone the project
* Run the test.py file to see the predicted result based on pickled train models.

