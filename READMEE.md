# KMeans Clustering on Breast Cancer Dataset

This project demonstrates how to perform KMeans clustering on the Breast Cancer Wisconsin dataset from scikit-learn.

## Overview

Clustering is an **unsupervised learning** technique used to group similar data points based on their features. KMeans requires specifying the number of clusters (`k`) beforehand. This project explores how to select an optimal `k` using two common methods:

- **Elbow Method:** Looks at the sum of squared distances (inertia) within clusters to find a point where adding more clusters yields diminishing returns.
- **Silhouette Score:** Measures how well each data point fits into its cluster compared to other clusters; higher scores indicate better-defined clusters.

The code evaluates `k` values from 2 to 10, selects `k=3` based on these metrics, performs clustering, and visualizes the results.

## Why Clustering?

In this context, clustering helps group patients with similar characteristics (e.g., tumor size, cell features) without using their diagnostic labels. The clusters may hint at different underlying conditions but do not directly correspond to specific diagnoses like "good", "medium", or "bad" health status.

## Features

- Load the Breast Cancer dataset (features only)
- Compute inertia and silhouette scores for k=2 to 10
- Visualize Elbow and Silhouette graphs to choose optimal k
- Perform KMeans clustering with k=3
- Visualize clusters on first two features with cluster centers
- Plot silhouette values for individual samples to assess clustering quality

## Requirements

- Python 3.x
- numpy
- pandas
- matplotlib
- scikit-learn

Install dependencies using:

```bash
pip install numpy pandas matplotlib scikit-learn
