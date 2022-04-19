# RANDOM CLASSIFICATION
# AIM:
  To write a python program to perform random classification.
# EQUIPMENTS REQUIRED:
  1.	Hardware – PCs
  2.	Anaconda – Python 3.7 Installation / Google Colab /Jupiter Notebook
# RELATED THEORITICAL CONCEPT:
  Random classifier: It creates a set of decision trees from randomly selected subset of training set. It then aggregates the votes from different decision trees to     decide the final class of the test object. Random Forest is suitable for situations when we have a large dataset, and interpretability is not a major concern.
  
  Purpose of Random classifier: One of the most important features of the Random Forest Algorithm is that it can handle the data set containing continuous variables as   in the case of regression and categorical variables as in the case of classification.
# ALGORITHM:
  1.	In Random forest n number of random records are taken from the data set having k number of records.
  2.	Individual decision trees are constructed for each sample.
  3.	Each decision tree will generate an output.
  4.	Final output is considered based on Majority Voting or Averaging for Classification and regression respectively.
# PROGRAM:
  /* 
  Program to implement random classification.
  
  Developed by   : ALLA VENKATA CHARAN REDDY
  
  Register Number : 212219040010 
*/ 

import matplotlib.pyplot as plt
from sklearn import datasets
X, y = datasets.make_blobs(n_samples=100,n_features=2,centers=2,cluster_std=1.05,random_state=2)
#plotting
fig=plt.figure(figsize=(10,8))
plt.plot(X[:, 0][y == 0], X[:, 1][y==0], 'r^')
plt.plot(X[:, 0][y == 1], X[:, 1][y==1], 'bs')
plt.xlabel("feature 1")
plt.ylabel("feature 2")
plt.title("Random Classification Data with 2 classes")
  
 # OUTPUT:
 ![image](https://user-images.githubusercontent.com/102689666/164060258-8ab94858-ac7c-459e-9a69-52d592c3931c.png)

 # RESULT:
  Thus, the Random Classification was successfully implemented using python programming.
