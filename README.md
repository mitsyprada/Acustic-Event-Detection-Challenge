# aml-aed-challenge-mitsyprada

 

# AEDC 

Main research question:

```
Can we infer the source of a sound recording from the tract and E (dB) data?
```

​	Yes, we can. Throughout the Acustic Event Detection Challenge ipynb file this is demonstrated calculating features sets obtained from this data, which are saved in the train_test_AEDC folder, in the form of h5py files. These feature sets are later used in 3 different algorithms: SVM (Support Vector Machine), k-means and HAC (Hierarchical Agglomerative Clustering). Results and discussion can be seen at the end of the document in the "Conclusions" section.

Subquestions:

```
1.How can we, based on the tract and E data, define a suitable set of features?
Which algorithms can be used to solve this task?
2.How does performance of the classifiers built depend on the machine learning algorithm and their parameters?
3.How does performance of the classifiers built depend on feature extraction parameters?
```

1. I need to feed my algorithms with features that define as precise as  possible the characteristic frequencies of the classes. I will take each file, slice the f_tract, s_tract and E features into three arrays each, leaving out the rows of zeros of s_tract, f_tract and E. Then I will  create histograms with appropriate frequency limits. To know those limits I took one of the classes (dog) and I analyzed the average maximum and  minimum frequencies, and plotted 5 histograms to make the decision of the range of the histograms used for the feature sets. The algorithm can be seen in the "Feature sets construction" section

2. This can be seen in the "Conclusions" section at the end of the Acustic Event Detection Challenge ipynb file.
3. This can be seen in the "Conclusions" section at the end of the Acustic Event Detection Challenge ipynb file.