# Recommender System Challenge 2021

[![Kaggle](https://img.shields.io/badge/open-kaggle-blue)](https://www.kaggle.com/c/recommender-system-2021-challenge-polimi)

This repository contains the source code for the 2021 Polimi Recommender System Challenge on [kaggle](https://www.kaggle.com/c/recommender-system-2021-challenge-polimi).

The goal of the competition was to create the recommender system for TV programs by providing 10 recommended products to each user. 

## Data

Given the User Rating Matrix and four Item Content Matrices we had to recommend 10 relevant tv shows to the users. 

The URM contained 5M interactions, 13650 users and 18059 item and a sparsity of 97.86 %.

The ICMs contained information about the channels, episodes, genre and subgenre of the shows.

## Recommender

My final recommender was a hybrid, obtained combining of the following models:
* S SLIM ElasticNet
* RP3Beta  


The hybrid combining S SLIM and RP3Beta merges their similarity matrices with a weighted sum. 

## Evaluation
The evaluation metric was MAP@10.

## Credits
This repository contains code from the [course framework repo](https://github.com/MaurizioFD/RecSys_Course_AT_PoliMi), that provides recommender implementations and utility code. 
Some code was taken from [this repo](https://github.com/Alexdruso/recsys-challenge-2020-polimi).

