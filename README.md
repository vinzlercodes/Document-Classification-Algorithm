# Document-Classification-Algorithm

Title: **Document Classification using Hierarchical Attention Networks**

Author: 
* Vinayak Sengupta (vs4016@rit.edu)


About:

In this repository, we use 50,000 IMDb movie reviews, specially selected for sentiment analysis, as well as a newly-adapted version of a [Paper](https://www.cc.gatech.edu/~dyang888/docs/naacl16.pdf), written by Yang et al. from the 2016 NAACL called Hierarchical Attention Networks for Document Classification.

## Contents

* **Document_Classifier.ipynb** - This notebook contains, the actual modelling of the Hierarchial Attention Network, it then takes in the data (avalialble in the data folder) and utilisng the model classifies sentences in the document and assigns attention values (more attention = sentence is important for classification of the document, less attention = sentence is not very important for classification of the document).
* **Sentence_Classifier.ipynb** - This notebook contains, the actual modelling of the Hierarchial Attention Network, it then takes in the data (avalialble in the data folder) and utilisng the model classifies words in the sentences of the document and assigns attention values (more attention = sentence is important for classification of the sentence and ultimately the document, less attention = sentence is not very important for classification of the sentence and ultimately the document).
* **Data** - The folder consists of the raw data set used.

## Requirements

* Python 3
* numpy
* pandas
* BeautifulSoup
* Matplotlib
* tensorflow
* keras
* (optional) CUDA cores

## How to Run
* Clone the project
* 

## Dataset

An analysis of 50,000 IMDB movie reviews was conducted for the labeled data set. Reviews are scored as binary sentiment, so a 5-star IMDB rating results in a score of 0, and a rating >=7 results in a score of 1. The sentiment of reviews is derived from what is written about each movie. It does not contain any movies that are part of the test set with 25,000 reviews. Furthermore, IMDB reviews without labels are available for another 50,000 titles.

## Models used
* Hierarchical Attention Network for Sentence Classification

<img height="600" src=https://user-images.githubusercontent.com/34100245/145495765-b46bc3ae-33e2-44ee-9556-73a1dcc36786.png />

* Hierarchical Attention Network for Word Classification

<img height="550" src=https://user-images.githubusercontent.com/34100245/145495832-395349bd-36b9-458a-84ff-727228b75f05.png />


## Result

* Hierarchical Attention Network for Document Classification

![download2](https://user-images.githubusercontent.com/34100245/145504812-d225823d-acf3-48cb-b5e3-9ab8cbb70563.png)

* Document Classification

![download (3)](https://user-images.githubusercontent.com/34100245/145504727-231fdf5e-d7be-4170-8ad8-d1f15fc66d80.png)


* Hierarchical Attention Network for Sentence Classification

![download](https://user-images.githubusercontent.com/34100245/145496222-f46d78fe-613e-49de-8dd9-e38779250444.png)

*  Sentence Classification

![download (2)](https://user-images.githubusercontent.com/34100245/145496426-fd09ff4d-072a-428c-9f20-53cb3a778dd3.png)

|Author | Model | Data Set | Accuracy |
|--- | --- | --- | --- |
|Yang et al. | HN-ATT | IMDB |49.4|
|Vinayak (me) | HN-GRU | IMDB |88.4  | 
|Vinayak (me) | HN-GRU  | IMDB |84.4 |

