# face_recognition_project

This is one of the projects I work on as I follow Aurelien Geron's Hands-On Machine Learning with Scikit-Learn, Keras and TensorFlow, Copyright 2019 Aurélien Géron, 978-1-492-03264-9. You can get yourself a copy of the book [here](https://www.amazon.com/Hands-Machine-Learning-Scikit-Learn-TensorFlow/dp/1491962291).

## The dataset

The clasic Olivetti faces dataset contains 400 grayscale 40x40-pixel images of faces. Each image is flattened to a 1D vector size of 4096. 40 different people were photographed (10 times each), and the usual task is to train a model that can predict which person is represented in each picture.


## Project scope

In this project, we will try to make a face recognizer, training and tuning a classifier and using different clustering and dimensionality reduction algorithm to boost our results.

## Project overview 

* We fetched the data and split it into a train set, a validation set and a test set
* We preprocessed the data making every image have the mean grayscale level
* We reduced the dimensionality of the images using the PCA algorithm
* We clustered the images using K-Means and search for the best number of clusters k
* We tried to used the cluster algorithm to improve the performance of the Random Forest classifier but it didn't help us at all
* We used the Gaussian Mixture models and the dimensionality reduction algorithm to detect anomalies 
* We tuned the Random Forest using the Grid Search for finding the best hyperparameters

## Code and Resources Used 
**Python Version:** 3.7  
**Packages:** pandas, numpy, sklearn, matplotlib  
**ML Book:** https://www.amazon.com/Hands-Machine-Learning-Scikit-Learn-TensorFlow/dp/1491962291


## Training Process 

* K-Means
* PCA
* Gaussian Mixtures
* Pipelines
* Grid Search 
* Random Forest

## Results

We observed that clustering the images in the Olivetti faces dataset didn't helped us improving the classifier, but the PCA and Gaussian Mixtures could've spotted the outliers easily. However, we were able to tune the Random Forest to 90% accuracy on the test set.



