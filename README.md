# K-Means-Clustering
K-Means Clustering on FIFA 22 Players

This project applies K-Means clustering to the FIFA 22 player dataset to discover natural groups of players based on performance, market value, wages, and age. It includes both a scratch implementation of K-Means and validation using scikit-learn.

# Project Overview
•	Goal: Segment FIFA 22 players into meaningful categories (e.g., stars, rising talents, prospects, role players).
•	Dataset: FIFA 22 player data (players_22.csv).
•	Features used:
   •	overall (current skill rating)
   •	potential (future ceiling)
   •	value_eur (market value)
   •	wage_eur (weekly wages)
   •	age

# What is K-Means?
K-Means is an unsupervised learning algorithm that groups data into k clusters based on similarity.
It works by iteratively:
Initializing cluster centers (centroids).
Assigning each player to the nearest centroid.
Updating centroids as the mean of assigned players.
Repeating until centroids stabilize.
The goal is to minimize within-cluster variance, so players within a cluster are as similar as possible.

# Steps in the Notebook

Data preparation
Load FIFA dataset, select key features.
Handle missing values and normalize data to a [1–10] scale for fair comparison.

Scratch implementation
Custom Python functions for centroid initialization, label assignment, centroid update, and iteration.
Visualization of clustering progress using PCA (2D reduction).

Cluster interpretation
Final cluster centers analyzed to understand group characteristics.
Example player names printed for each cluster.

Validation with scikit-learn
Run sklearn.cluster.KMeans with the same data.
Compare centroids and assignments with the scratch version.
