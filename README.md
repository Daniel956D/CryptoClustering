# Cryptocurrency Clustering Analysis
Module Challenge 11 

## Overview
This project applies unsupervised learning techniques to analyze cryptocurrency market data. Using Python and scikit-learn, the analysis employs K-means clustering and Principal Component Analysis (PCA) to identify patterns in cryptocurrency price movements.

## Technologies Used
- Python 3.x
- Pandas for data manipulation
- scikit-learn for machine learning algorithms
- Matplotlib for data visualization

## Analysis Process
1. Data Preprocessing
  - Loaded cryptocurrency market data
  - Normalized data using StandardScaler
  - Prepared data for clustering analysis

2. K-means Clustering
  - Applied elbow method to find optimal number of clusters
  - Implemented K-means clustering on original scaled data
  - Visualized results using scatter plots

3. Principal Component Analysis (PCA)
  - Reduced features to three principal components
  - Achieved 99.98% explained variance ratio
  - Applied K-means clustering on PCA-transformed data

## Results
- Optimal clusters identified: 4
- PCA explained variance: 99.98%
- Successfully grouped cryptocurrencies based on price change patterns

## Code Sources and References
- Scikit-learn Documentation:
 - [K-means Clustering](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html)
 - [Principal Component Analysis](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)
 - [StandardScaler](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html)

- Analysis code structure adapted from:
 - Scikit-learn clustering examples: [Clustering Documentation](https://scikit-learn.org/stable/modules/clustering.html)
 - Python Data Science Handbook by Jake VanderPlas (O'Reilly Media)

## Installation
```python
# Required libraries
import pandas as pd
import numpy as np
from sklearn.preprocessing import StandardScaler
from sklearn.decomposition import PCA
from sklearn.cluster import KMeans
import matplotlib.pyplot as plt
