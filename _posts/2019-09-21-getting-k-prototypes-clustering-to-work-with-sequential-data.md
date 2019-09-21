---
layout: post
title: Getting K-Prototypes Clustering to Work with Sequential Data
date: 2019-09-21 02:52
categories:
author: Kawsar Noor
---

Sequential data is all around us. Consider web traffic data for a single user. The data would perceivably contain a time seperated sequence of events that the website was interested in recording. (e.g where on the page the user was or what buttons they were pressing etc). This sequence serves as quite a useful profile of user behaviour and acts as a type of fingerprint for the user.

When many sequences are compared against each other patterns begin to emerge and we can begin to build up a picture of similar sequences. This of particularly useful in cases where we want to cluster together sequences.

## Clustering Heteregenous Data Types
Now most clustering algorithms are suited for datasets using homogenous variables. K-means for example demands an all numerical dataset as they make use of an averaging function. K-modes for example is useful for categorical datasets and makes use of binary counts.

K-prototypes was an algorithm Zhang which allowed a for a distance measure that combined aspects of both K-means and K-modes. The idea is that in order to calculating the differences in categorical data we would use the distribution of differences in the numerical dataset to give us a weighting that we could then apply. Zhao proposed using the standard deviation of the numerical attributes.

In essence it means that if there is a mismatch in categorical data it is weighted according to the average standard deviation of the numerical dataset which is denoted as $$\gamma$$ Although there were later proposals to update the

$$
d(X,Y) = \sum(x_j - y_j)^2 + \gamma \sum \delta(x_j, y_j)
$$

## Working with Mixed Length Data
As we have seen the K-prototypes algorithm is set up to work with data of a consistent dimensionality. In this section we'll take a look at modelling sequential data using a mixture of numerical and categorical types.

Consider the example of a mobile app user. We are collecting user experience data and are monitoring the amount of time the user spends in various parts of our app. To keep things simple let's assume we have three interactive widgets in our app which we'll call $$w = \{w_1, w_2, w_3\} $$. Each user interacts with a widget abstains for a portion of time and interacts with another widget or even the same widget. So a user-sequence may look like:

$$
s_1 = (w_1, 20, w_2, 30, w_3....)
\\
s_2 = (w_3, 10, w_2, 10, w_3....)
$$

### Distance Measure for Mixed Length Data
