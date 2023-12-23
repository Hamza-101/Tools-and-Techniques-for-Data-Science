# Instructions: 
## The aim of this assignment is to give  understanding of basic clusterings such as k-means and DBSCAN. 

Say you are given a data set where each observed example has a set of features, but has no labels. Labels are an essential ingredient to a supervised algorithm like a Decision Tree or Random Forest, which learns a hypothesis function to predict labels given features. So we can't run supervised learning. What can we do? 
One of the most straightforward tasks we can perform on a data set without labels is to find groups of data in our dataset which are similar to one another -- what we call clusters.  K-means and DBSCAN are among the most popular "clustering" algorithms. In this assignment, we will compare these algorithms.  

Your task is to: 

1.	Perform basic preprocessing on the Breast cancer dataset.
    a.	Drop the label columns while making clusters as in clustering we do not have labels. We will use these labels to evaluate the performance of the models so do not drop labels permanently
    
    b.	If there are any categorical variables, perform one-hot encoding. Otherwise, scale data using Min-Max Scaler. 
    
    c.	Perform PCA on data and visualize data samples using 2D scatter plot. Plot samples of each class with different colors.
    d.	You can remove outliers and noise.
    
    e.	Remove irrelevant columns 
    
    f.	Perform EDA to see for which class most sample exists in the data (save this information and use it for assigning cluster labels)


2.	Write functions for the K-means algorithm from scratch. You can not use built-in ML libraries such as sklearn for this task. For basic operations, you can use NumPy and similar libraries only. You can use online references and lectures to understand the concepts but write your own code. Your code should be in modular form and can be generalizable (such as we can change parameters or dataset).

 
3.	Perform clustering using the K-means algorithm (only create 2 clusters) using all features, save these cluster labels, and plot the data (on which you performed PCA) but now use clustering labels to assign a color to each sample. Assign each sample a label according to cluster size. For example, if a sample is from larger clusters assign it a label of the class having more samples in the data, and so on. Use these labels as predicted labels.

   
4.	Use predicted labels and actual labels to evaluate the performance of the clustering algorithm. Show accuracy, precision, recall, f1, and confusion report.

   
5.	Now use the built-in function for K-means clustering from sklearn and repeat step 3 and 4 and compare the outcomes.
    
6.	Now use the built-in DBSCAN algorithm (such as from sklearn) and repeat step 3 and 4 and compare the outcomes with other experiments.
    
7.	Report your findings in a paragraph in the same notebook using a markdown cell.
    
8.	Bonus task: You can compare the clusters and performance before applying PCA to data and after applying PCA to see the impact of dimensionality reduction on clustering.
