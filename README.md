# Recommender System Challenge 2021

[![Kaggle](https://img.shields.io/badge/open-kaggle-blue)](https://www.kaggle.com/c/recommender-system-2021-challenge-polimi)

This repository contains the source code for the 2021 Polimi Recommender System Challenge on [kaggle](https://www.kaggle.com/c/recommender-system-2021-challenge-polimi).

The goal of the competition was to create the recommender system for TV programs by providing 10 recommended products to each user. 

## The Competition

Goal:

The application domain is TV programs recommendation. The datasets we provide contains both interactions between users and TV shows, as well as features related to the shows. The main goal of the competition is to discover which items (TV shows) a user will interact with.
Each TV show (for instance, "The Big Bang Theory") can be composed by several episodes (for instance, episode 5, season 3). The goal of the recommender system is not recommend a specific episode, but to recommend the TV show.

Description:

The datasets includes around 6.2M interactions, 13k users, 18k items (TV shows) and four feature categories: 8 genres, 213 channels, 113 subgenres and 358k events (episode ids).
The training-test split is done via random holdout, 85% training, 15% test.
The goal is to recommend a list of 10 potentially relevant items for each user. MAP@10 is used for evaluation. You can use any kind of recommender algorithm you wish e.g., collaborative-filtering, content-based, hybrid, etc. written in Python.

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

