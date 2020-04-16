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
    - [Features](#feature importance)
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

<img width="783" alt="Screen Shot 2020-04-11 at 12 24 31 AM" src="https://user-images.githubusercontent.com/52756457/79397952-06191700-7f45-11ea-8dcf-5267a184f705.png">

The graph above shows us the important feaures in the model.



![Screen Shot 2020-04-15 at 6 08 29 PM](https://user-images.githubusercontent.com/52756457/79398289-edf5c780-7f45-11ea-86ca-36eed925b9c2.png)

The graph above shows the number of total crimes reported monthly throught the year 2016. We can see the increase in number of crimes being comitted from 06-2016 - 11-2016.


![Screen Shot 2020-04-15 at 6 01 56 PM](https://user-images.githubusercontent.com/52756457/79398409-44fb9c80-7f46-11ea-9498-5d97b10b6343.png)

The graph above shows the total number of arrest made monthly. We can see how the number of arrest steadily drops after 07-2016. I wonder why that is happening because around the same time the overall number of crimes increase. So one would assume the number of arrest made should increase as well. However that is not that case for this dataset.  

### Modeling <a name="modeling"></a>
I used these Machine Learning Algorithms for modeling my data.
- Decision Tree
- AdaBoost
- Gradient Boosting
- XG Boost
- Random Forest

### Features  <a name="feature importance"></a>

<img width="783" alt="Screen Shot 2020-04-11 at 12 24 31 AM" src="https://user-images.githubusercontent.com/52756457/79397952-06191700-7f45-11ea-8dcf-5267a184f705.png">


These are some of the features that went into making my model. It suprised to see how some features are more important than others when it comes to predicting arrest. It was very interesting to see that Percent over 25 without high school diploma is the 2nd most important feature. It shows majority of people arrest lack education. This is something that should be looked into more.