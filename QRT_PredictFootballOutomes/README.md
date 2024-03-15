# Competition submission hosted by Qube Research & Technologies

## Description
QRT is a prop trading firm, and they provided datasets from football matches in order for competition participants to predict the outcome of a 
football match given some data. Overall objective was a 3-class classification problem with XGBoost as the benchmark.

## Approach
My approach to beating the benchmark was 3-fold: (1) preprocess the data, (2) use AdaBoost, (3) optimize AdaBoost. The idea behind this approach
was that more finely preprocessing the data would allow me to utilize all the data, and AdaBoost would combine pre-existing weak learners into one,
final strong learner that would beat XGBoost.

## Relevant Statistics
1. Train_test split accuracy on test set (Benchmark **47.42%**, optimized AdaBoost **70.66%**)
2. Private dataset by QRT (Benchmark public leaderboard **45.65%**, optimized AdaBoost **46.89%**)
3. #1 Ranked model 49.27% - **Difference of 2.38%**

