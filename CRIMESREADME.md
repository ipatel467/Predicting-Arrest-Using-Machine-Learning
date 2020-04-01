# Predicting Arrest
###### By Ibrahim Patel

![](https://media.giphy.com/media/hc1lHJaHoSPAc/giphy.gif)


## Executive Summary
I gathered my data from an open source called Chicago Data Portal. With this source I got 2 datasets on crime and socioeconmic staus. I began to answer some of the many questions I had about crime. However, many other questions would arise. It is my goal to make a machine learning algorithm that can predict whether an arrest is made or not.

## Contents
1. [Introduction](#introduction)
    - [Problem Statement](#problem_statement)
    - [Dataset](#dataset)
2. [Analysis](#analysis)
    - [Data Cleaning](#data_cleaning)
    - [Exploratory Analysis](#exploratory_analysis)
    - [Modeling](#modeling)

## Introduction <a name="introduction"></a>

### Problem Statement <a name="problem_statement"></a>
Crime is a very relative topic, and the problem is that crime harms the community as a whole. There are millions of crimes reported and committed, however, only around 20% of those crimes result in an arrest. I wanted to see if I could make a model that can predict whether an arrest was made or not on a crime. I am using the a dataset with the crime from my home city just to make it a little more interesting for me.
### Dataset <a name="dataset"></a>
Chicago Data Portal

https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-present/ijzp-q8t2

## Analysis <a name="analysis"></a>

### Data Cleaning <a name="data_cleaning"></a>

I merged 2 different dataframes, dropped null and missing values, and I dropped any duplicated or unwanted values. 

### Exploratory Analysis <a name="exploratory_analysis"></a>

I found that location, education, and harship index  have the highest effect on whether an arrest is made or not. I also found out that crime is very seasonal as I saw the trends repeat themselves over the years. Crime tend to peak during the summer months, and crime drops greatly in the winter season.

### Modeling <a name="modeling"></a>
I used these Machine Learning Algorithms for modeling my data.
- Decision Tree
- AdaBoost
- Gradient Boosting
- XG Boost
- Random Forest



