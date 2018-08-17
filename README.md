# Deloitte_March_Data_Crunch_Madness
AN OPTIMIZED MACHINE LEARNING MODEL FOR PREDICTING 2018 MARCH MADNESS GAMES RESULT

Team name: Orange

Team member: Yichen Pan, Ziyue Zhong, Haojunzhi Yu, Tina George

Introduction

The National Collegiate Athletic Association (NCAA) Men's Basketball Tournament is informally referred to as "March Madness." With 68 college basketball teams competing in a single-elimination tournament, March Madness is played every spring in the US to determine the national championship of the major college basketball teams. Based on Kaggle’s Machine Learning Mania(https://www.kaggle.com/c/mens-machine-learning-competition-2018#evaluation ), competitors of 2018 Deloitte March Data Crunch Madness predict the probability that a team wins any given game in the 2018 Tournament. Log loss is used as evaluation. Extensive historical data to jump-start the modeling process is given. Competitors are encouraged to incorporate their sources of data.

Highlights of Our Project

One of the highlights of our project is the new variables, including EFG-OEFG, TPP-DTPP, SRS, SOS, Adj_win and the most important one Coach Influence. Another one is our project's philosophy, let the machine learning algorithm decide variables and models. We try to make all procedures rational and scientific. 

First, I want to show our project flow. 

![picture](https://github.com/hoddiemelo/March_Data_Crunch_Madness/blob/master/flow%20chart.jpg)

The first step is Data Processing including data collection and data cleaning. In this part, we add several essential variables.

![picture](https://github.com/hoddiemelo/March_Data_Crunch_Madness/blob/master/addvariables.jpg)

We created a new variable named Coach Influence. The way how we make it is on the below.

![picture](https://github.com/hoddiemelo/March_Data_Crunch_Madness/blob/master/Coach%20Influence.jpg)

Also, the descriptive analysis indicates the difference between teams home win% and away win%. So I made the adjusted win formula.

![picture](https://github.com/hoddiemelo/March_Data_Crunch_Madness/blob/master/Adjusted%20Win.jpg)

And then feature selection, we applied three feature selection methods (L1-based feature selection, Tree-based feature selection, and Pearson correlation linear feature selection). We measured the performance of Ensemble model by using data selected by all three feature selection methods. The testing score and testing log loss indicate that variables chosen by L1-based feature selection have the best performance.

![picture](https://github.com/hoddiemelo/March_Data_Crunch_Madness/blob/master/FeatureSelection.png)

We compared the performance of all eight models measured by testing score and testing gloss. According to this result, we selected LogisticRegression, RandomForest, Gradient boosting and Decision Tree to predict the outcome by using Ensemble Model VotingClassifier.

![picture](https://github.com/hoddiemelo/March_Data_Crunch_Madness/blob/master/Testing%20Score.png)

![picture](https://github.com/hoddiemelo/March_Data_Crunch_Madness/blob/master/Testing%20log%20loss.png)

In the end, I'd like to show our model performance in predicting 2018 March Madness. This chart shows our prediction distribution and correctness. We finally get 74.6% accuracy (successfully predicted 50 of 67 games)and log loss 0.58

![picture](https://github.com/hoddiemelo/March_Data_Crunch_Madness/blob/master/2018%20Prediction%20probability%20distribution%20and%20correctness.jpg)






