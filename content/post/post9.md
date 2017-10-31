+++
showonlyimage = true
draft = false
date = "2017-10-23T18:25:22+05:30"
title = "K Nearest Neighbors"
weight = 0
+++

K Nearest Neighbors

K nearest Neighbors is a classification algorithm that uses similar characteristics  to give labels to unlabeled data. The advantages of K nearest neighbors include that is very simple and that it does not make any assumptions about the data. The disadvantages include that it is not very effective when the data is noisy and when there are clear boundaries between groups. Additionally it does not leave the analyst with a model, and selecting the wrong K can lead to inaccuracies.

The K in K nearest neighbors refers to the number of neighbors that the analyst chooses to classify as part of a class. The algorithm identifies k observation in the training data nearest in proximity. The algorithm uses distance to measure similarity. This distance can be calculate in several ways including Euclidean and Malahanobis among others.

Choosing the right K can be difficult. A large K can result lower impact of variance on error, but can run the risk of ignoring important patterns in the data. However choosing a small K can make noisy data or outliers negatively impact the accuracy of the algorithm.

KNN can take different types of data and can predict ordinal or nominal data. Before using the algorithm, it is necessary to normalize all the variables. However, KNN gives you no model.


