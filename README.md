# Pokémon Categorisation Project
## Overview
This project is a fun exploration that categorises Pokémon based on their statistical attributes, including attack, defence, special attack, special defence, speed, and HP. The goal is to analyse and group Pokémon using machine learning techniques, specifically K-means clustering and DBSCAN.

## Dataset
The dataset used for this project is sourced from Kaggle and can be downloaded [here](https://www.kaggle.com/datasets/rounakbanik/pokemon?resource=download). It contains 41 columns, but this project focuses on the following features:
- `name`: The English name of the Pokémon
- `pokedex_number`: The entry number of the Pokémon in the National Pokédex
- `attack`: The Base Attack of the Pokémon
- `defence`: The Base Defence of the Pokémon
- `sp_attack`: The Base Special Attack of the Pokémon
- `sp_defence`: The Base Special Defence of the Pokémon
- `hp`: The Base HP of the Pokémon
- `speed`: The Base Speed of the Pokémon
- `generation`: The numbered generation in which the Pokémon was first introduced
- `is_legendary`: Indicates if the Pokémon is legendary


## Methodology
### Clustering Techniques
1. **K-means Clustering**
   - Used to partition the Pokémon into distinct clusters based on their stats.
   - The number of clusters was determined using the elbow method.
2. **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**
   - Utilised to find clusters based on density, allowing for the identification of outliers.

### Evaluation
The performance of the clustering algorithms was evaluated using the **Silhouette Coefficient**, which measures how similar an object is to its own cluster compared to other clusters. A higher silhouette score indicates better-defined clusters.

# File structure
* `data/pokemon.csv`: dataset for analysis
* `main.ipynb`: An analysis of the status of Pokémon