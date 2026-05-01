# spotify-clustering-project

## Setup
pip install -r requirements.txt

## How to run
1. Open notebooks/data cleaning.ipynb for data cleaning/database
2. Open notebooks/clustering.ipynb for clustering model and recommendation
3. Run all cells from top to bottom

# Audio Feature Clustering Analysis

## Research Question
Do clusters formed from audio features correspond to overall moods?

## Purpose
This project investigates whether unsupervised machine learning (K-means clustering) can discover 
mood labels associated in songs using only audio features, without any specified mood labels as input.

## What I Did
- Cleaned and stored song data in a SQLite database
- Selected and normalized audio features (e.g. tempo, energy, valence, etc)
- Applied K-Means clustering with k=4 chosen via the elbow method/silhouette score
- Evaluated clusters using silhouette score and stability analysis
- Visualized clusters with PCA and heatmaps
- Built a recommendation system using cosine similarity