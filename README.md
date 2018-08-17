# Deloitte_March_Data_Crunch_Madness
AN OPTIMIZED MACHINE LEARNING MODEL FOR PREDICTING 2018 MARCH MADNESS GAMES RESULT

Team name: Oragne

Team member: Yichen Pan, Ziyue Zhong, Haojunzhi Yu, Tina George

Introduction

The National Collegiate Athletic Association (NCAA) Men's Basketball Tournament is informally referred to as "March Madness". With 68 college basketball teams competing in a single-elimination tournament, March Madness is played every spring in the US to determine the national championship of the major college basketball teams. Based on Kaggle’s Machine Learning Mania(https://www.kaggle.com/c/mens-machine-learning-competition-2018#evaluation ), competitors of 2018 Deloitte March Data Crunch Madness predict the probability that a team wins any given game in the 2018 Tournament. Logloss is used as evaluation. Extensive historical data to jump-start the modeling process is gived. Competitors are encouraged to incorporate their own sources of data.

Highlights of Our Project

One of the highlight of our project is the new variables, including EFG-OEFG, TPP-DTPP, SRS, SOS, Adj_win and the most important one Coach Influence. Another one is our project's philosophy, let the marchine learning algorithm decide variables and models. We try to make all procedures become rational and sentific. 

First, I want to show our project flow. 

The first step is Data Processing including data collection and data cleaning. In this part we add several important variables.

We create a totally new variable named Coach Influence. The way how we make it is on the below.

And then feature selection, we applied three feature selection methods (L1-based feature selection, Tree-based feature selection and Pearson correlation linear feature selection). We measured the performance of Emsemble model by using data selected by all three feature selection methods. The testing score and testing logloss indicates that variables selected by L1-based feature selection have the best performance.

We compared the performance of all eight models mearsured by testing score and testing logloss. According to this result we selected LogisticRegression, RandomForest, GradientBoosting and Decision Tree to emsemble the result.



![picture](https://github.com/hoddiemelo/March_Data_Crunch_Madness/blob/master/added_variables.jpg)
