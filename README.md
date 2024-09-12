# Instagram Followers, Following, and Close Friends Analysis Using Bayesian Models

This project evaluates the relationship between Instagram followers, the number of accounts followed, and the number of close friends. The analysis is conducted using Bayesian models, specifically through OpenBUGS and MCMC (Markov Chain Monte Carlo) methods, to provide robust insights on how these factors influence a user's number of followers.

## Table of Contents
- [Introduction](#introduction)
- [Data Collection](#data-collection)
- [Methodology](#methodology)
- [Results](#results)

## Introduction
This project seeks to understand how the number of followers on Instagram is related to two main factors:
1. The number of accounts a user follows.
2. The number of close friends a user has.

Using Bayesian approaches, we analyze the relationships between these variables and determine the strength and significance of their influence on follower count.

## Data Collection
Data was collected through a Google Form where respondents answered three main questions:
- How many followers do you have?
- How many accounts do you follow?
- How many people are in your Close Friends list on Instagram?

The dataset was then cleaned and preprocessed by removing outliers and irrelevant columns and converting all values to integers.

## Methodology
The analysis was performed using the following steps:
- **Data Preprocessing**: Removing outliers, erasing values where all three columns are zero (indicating no Instagram account), and converting values to integers.
- **Exploratory Data Analysis**: Scatter plots were generated to show relationships between followers, following, and close friends, as well as distribution histograms for each variable.
- **Frequentist Approach**: Linear regression was applied to explore how well the number of followers can be predicted by the number of close friends and accounts followed.
- **Bayesian Analysis**: 
  - **MCMC**: Markov Chain Monte Carlo simulations were used to estimate the posterior distribution of followers.
  - **OpenBUGS**: A Bayesian regression model was constructed using OpenBUGS to further investigate the relationships.

## Results
The analysis yielded the following insights:
- **Followers vs Following**: A strong positive correlation between the number of followers and accounts followed.
- **Followers vs Close Friends**: A moderate positive correlation, indicating that having more close friends increases the likelihood of more followers.
- **Bayesian Regression**: The Bayesian model confirmed the significance of both predictors (following and close friends) and provided credible intervals for follower predictions.
