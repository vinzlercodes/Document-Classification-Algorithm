# Document-Classification-Algorithm

Title: **Document Classification using Hierarchical Attention Networks**

Author: 
* Vinayak Sengupta (vs4016@rit.edu)


About:

In this repository, we use 50,000 IMDb movie reviews, specially selected for sentiment analysis, as well as a newly-adapted version of a [Paper](https://www.cc.gatech.edu/~dyang888/docs/naacl16.pdf) from the 2016 NAACL called Hierarchical Attention Networks for Document Classification.

## Contents

* **Document_Classifier.ipynb** - This notebook contains, the actual modelling of the Hierarchial Attention Network, it then takes in the data (avalialble in the data folder) and utilisng the model classifies sentences in the document and assigns attention values (more attention = sentence is important for classification of the document, less attention = sentence is not very important for classification of the document).
* **hatt_model.ipynb** - The notebook utilises the generated utility files from the previous file, along with different configurations as compared to the paper's (e.g. loss function, optimizer function, etc) trains, saves, and also evaluates the model with words' and sentences' weights visualizations.
* **Data** - The folder consists of the raw data set used along with the GLoVE embeddding file that has been utilised. 
* **Utilities** - The folder contains all the generated output files from data_preprocess.ipynb, so that we can directly feed them into hatt_model.ipynb.
* **Model_Weights** - 


## Requirements

* Python 3 (3.6)
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

## Models used
* Hierarchical Attention Network for Sentence Classification

<img height="600" src=https://user-images.githubusercontent.com/34100245/145495765-b46bc3ae-33e2-44ee-9556-73a1dcc36786.png />

* Hierarchical Attention Network for Word Classification

<img height="550" src=https://user-images.githubusercontent.com/34100245/145495832-395349bd-36b9-458a-84ff-727228b75f05.png />


## Result

* Hierarchical Attention Network for Document Classification



* Hierarchical Attention Network for Sentence Classification

![download](https://user-images.githubusercontent.com/34100245/145496222-f46d78fe-613e-49de-8dd9-e38779250444.png)

*  Sentence Classification

![download (2)](https://user-images.githubusercontent.com/34100245/145496426-fd09ff4d-072a-428c-9f20-53cb3a778dd3.png)




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
* 

