---
layout: post
title: Everything you ever wanted to know about t-SNE but were too afraid to ask
date: 2020-09-28 12:00:00 
description: An overview of the t-SNE algorithm, its advantages and its disavantages and how to use it in python # Add post description (optional)
img: croc.jpg # Add image post (optional)
fig-caption: Big ol' crocodile # Add figcaption (optional)
tags: [python, tsne, machine learning, scikit-learn]
---

# Why should I care

So you've got this dataset, and it has a lot of variables or attributes (or columns). Too many to begin to start thinking about. A staggeringly high numbers of variables, sometimes the number of variables, can exceed the number of observations (rows). In data science this is known as having a dataset with **high dimensionality**[^1]. 

In datasets with high dimensionality, its often difficult to do high level calculations, its even more difficult to get a feel for how the observations compare to each other. We are good however at doing this for datasets with low dimensionality. What we need to do is go from our difficult high dimensional dataset to an easy low dimensional dataset. This process is called **dimensionality reduction**[^1], and of course there are way too many ways to do it.

[image]

Step in the big kahuna of the dimensionality reduction world **Principle Component Analysis** or **PCA** for short.

## I'm already bored

There's a reason you don't get many mathematicians in marketing departments, but behind the dull as bricks name is a clever algorithm. What PCA does is take our large high dimensionality dataset and convert it into a low dimensionality dataset **whilst still retaining most of the information!** We can go from a 3000 column dataset to a 2 column dataset with a minimal loss our ability to measure how the observations relate to each other.

## Lots of numbers to less numbers, big whoop

Alright, let's look at an example. Lets run a PCA on something nice with no risk of being controversial. This is the voting record for all of the UK Members of Parliament from 2010 to 2015[^2]. 

![A pandas dataset showing the voting record of MPs. It is 664 rows (one per MP) and 1226 columns (one per bill).](./../assets/img/pca-mpvotes.png)

As you can see each members can vote on any number of bills, but the number of bills outnumbers the number of members. We're going to use PCA to see if we can pull out any structure that might be hiding in this dataset. 



# What should it do



# Why is it called that 



# What's in a name 

t-sne is an abbreviation of 't-distributed stochastic neighbor embedding'. Lets breakdown what that means. 

[^1]: https://www.statisticshowto.com/dimensionality/
[^2]: https://www.publicwhip.org.uk/

