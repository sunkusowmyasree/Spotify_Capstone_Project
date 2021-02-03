# Spotify_Capstone_Project

## Table of Contents
1. [Description](#description)
2. [Installing](#installing)
3. [Project Tasks](#Tasks)
4. [File Structure](#FileStructure)
5. [Medium Blog](#blog)
5. [Authors](#authors)
6. [License](#license)

<a name="descripton"></a>
## Description

This Project is a part of Data Science Nanodegree Program by Udacity.
The dataset is taken from Kaggle Website. 
The aim of the project is to build a ML model that can predict popularity of any song and also build a Recommendation system based which can recommend songs to any given song

<a name="installing"></a>
### Installing
There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python. The code should run with no issues using Python versions 3.*.

<a name="Tasks"></a>
### Project Tasks
Your project will be divided into the following tasks

I. Exploratory Data Analysis

First step is to explore the data you are working with for the project. Dive in to see what you can find. There are some basic, required questions to be answered about the data you are working with throughout the rest of the notebook. Use this space to explore, before you dive into the details.

II. ML Modelling

Before we start building a model for prediction. Let's first find the features which are highly correlated with Popularity feature and use them as feature variables that we will trained in the model.
Next will be performing Feature Transformations. The steps followed are 
* Object data of the artists with some numerical indicator that identify the artist.
* Eliminate Zero values from tempo columns and replace it
* Standardizing Instrumental Criteria with numeric values
* Using OneHotEncoder from SKlearn to create dummies
* Minmax Scaling for relevant features
* Target Scaling for Popularity Column

Below are a few models which I have attempted:
1. Decision Tree Regressor
2. Decision Tree with Grid Search CV
3. Random Forest Regressor (RF)

And  the best accuracy is achieved by Decision Tree with Grid Search CV model

III. Neighbourhood Based Collaborative Filtering Recommendation

Building a recommendation system where it recommends similar songs for any given song.

In this project I have used Neighbourhood Collaborative Filtering using similarity metrics method. Calculated Manhattan Distance using all numerical features available in the dataset and find the neighbour songs which have relatively less distance.

<a name="FileStructure"></a>
### File Structure

* `data` folder contains the following:
    * `data.csv`: contains the songs data csv file
    * `data_by_artist.csv`: contains the artist data csv file
    * `data_by_genres`: contains the genres data csv file
    * `data_by_year.csv`: contains the Year Wise data csv file
    * `data_w_genres.csv`: contains the data with genres csv file
  
* `Spotify_Capstone_Project.ipynb ` : Jupyter notebook with python codes

<a name="blog"></a>
### Results
The main findings of the code can be found at the post available [here]()

<a name="authors"></a>
## Authors

* [Sowmya](https://github.com/sunkusowmyasree/) | [LinkedIn](https://www.linkedin.com/in/sunku96/)

<a name="license"></a>

## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

