## Introduction :

Preprocessing is a mandatory step for prediction of instances in any data set. Preprocessing involves various steps but a concrete algorithm to do this preprocessing is very hard to find. In this projet we have discussed various methods aimed solely for removing any mislabelled or noisy data points from the data set. Various methods such as Adaboost, Clustering and Semi Supervised learning have been used in order to design an appropriate algorithm to carry out this preprocessing technique. The description of the various methods used is give below -:

1. Mode Method
2. Mean Method
3. Cluster based Boosting(only we visulized the data then we not went further .)
4. Clustering as a Feature
   5.Clustering as a Feature with Semi-Supervised Learning
5. Double Addition of Cluster in Semi-Supervised Learning

### below all are the classifire we used in this project

1. Adaboost(Ensemble Learning)
2. SVM
3. Decision Tree
4. Naive Bayes
5. Voting Classifire
6. Knn

## Prerequisite Concept:

1)Adaboost-:
AdaBoost, short for “Adaptive Boosting”, is the first practical boosting algorithm proposed by Freund and Schapire in 1996. It focuses on classification problems and aims to convert a set of weak classifiers into a strong one.In the adaboost ,it have N weak classifier .

Algorithm

1. weight vector(w) created of size N
2. In the first iteration all data point assign same weight ,so we assigned 1/N for all the N spaces of the weight vector .
3. The training data and corresponding weight will go to the weak classifier .
4. After that we will calculate following
   > 1. Error Rate(err) =sum{w(i) \* terror(i)} / sum(w)
   > 2. Alpha = 0.5\*(log(1 - err) - log(err))
5. Now update the weight list for the next iteration using this formula

> w(i)=w(i)*exp(-Alpha *y(i)\*y_pred(i)

**Where y(i)=actual label value at i instance and y_pred(i)=Predicted label value by model at i instance**

6. Normalize the weight list using w(i)=w(i)/sum(w(i))
7. Again start from the 3 ,till a better accuracy not get by model.

### Detailed report available at [this link](https://docs.google.com/document/d/e/2PACX-1vQaHD_xFcjkw1IsZwBLwXRe3J-Fek9LN-_CG8wYKeI8x_1UUDXE0hW7inIn11byjSJBD6z6WOpZQtxM/pub)

**Note: The code is avialble for only DATASET A and cluster based boosting code is incomplete right now**
