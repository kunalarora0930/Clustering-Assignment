# Clustering Utilizing Pycaret with Comparison of Various Preprocessing Approaches

## Overview

This document details an assignment where three different clustering techniques were applied to a dataset. The performance of these clustering algorithms was evaluated across various preprocessing methods and different numbers of clusters.

The three clustering methods employed are:

1. KMeans Clustering
2. Hierarchical Clustering
3. MeanShift Clustering

## Dataset

The dataset utilized is the **Anuran Calls (MFCCs)** dataset sourced from the UCI dataset library. This dataset comprises acoustic features extracted from syllables of frog calls, including labels for family, genus, and species.

- Number of Instances: 7195
- Number of Attributes: 25 + 1 (ID)

Originally created for tasks related to anuran species recognition through their calls, this dataset is multilabel and consists of three label columns. It comprises segments of 60 audio records from 4 different families, 8 genera, and 10 species. Each audio record corresponds to an individual frog specimen, with an additional column for record ID.

## Evaluation Metrics

Three metrics were employed to assess the performance of clustering algorithms:

1. **Silhouette Score**: Evaluates the clustering algorithm's performance based on the compactness of individual clusters (intra-cluster distance) and separation among clusters (inter-cluster distance). The score is calculated per sample and then averaged across all samples.

2. **Calinski-Harabasz Score**: Defined as the ratio of the sum of between-cluster dispersion to within-cluster dispersion.

3. **Davies-Bouldin Index**: A validation metric measuring the average similarity between each cluster and the cluster most similar to it. It assesses clusters based on the ratio between inter-cluster and intra-cluster distances.

## Results

Results for each clustering method are displayed below:

- KMeans Clustering
  ![KMeans Result](https://github.com/kunalarora0930/Clustering-Assignment/blob/main/Results/Kmeans.png)

- Hierarchical Clustering
  ![Hierarchical Result](https://github.com/kunalarora0930/Clustering-Assignment/blob/main/Results/Hierarchical.png)

- MeanShift Clustering
  ![MeanShift Result](https://github.com/kunalarora0930/Clustering-Assignment/blob/main/Results/Mean%20Shift.png)