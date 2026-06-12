# Netflix Recommendation System

## Overview

This project develops a personalized movie recommendation system using the Netflix Prize Dataset.

The objective is to learn user preferences from historical movie ratings and generate relevant recommendations for unseen movies.

Two recommendation approaches were implemented and compared:

* Item-Based Collaborative Filtering
* Singular Value Decomposition (SVD)

The final system generates Top-K movie recommendations and evaluates recommendation quality using RMSE.

---

## Dataset

Netflix Prize Dataset
https://www.kaggle.com/datasets/netflix-inc/netflix-prize-data?utm_source=chatgpt.com 

Contents:

* User ID
* Movie ID
* Rating
* Rating Date
* Movie Metadata

For computational efficiency, a subset of 3 million ratings was used.

---

## Methodology

### Exploratory Data Analysis

* Rating Distribution
* User Activity Analysis
* Movie Popularity Analysis
* Dataset Sparsity Analysis

### Recommendation Models

#### Item-Based Collaborative Filtering

Uses similarity between movies to generate recommendations.

#### Singular Value Decomposition (SVD)

Learns latent factors representing user preferences and movie characteristics.

---

## Results

| Model                              | RMSE   |
| ---------------------------------- | ------ |
| Item-Based Collaborative Filtering | 1.0723 |
| SVD                                | 0.9889 |

SVD achieved the best performance and was selected as the final recommendation model.

---

## Recommendation Generation

The final model predicts ratings for unseen movies and recommends the Top-10 movies with the highest predicted ratings.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Surprise
* Jupyter Notebook

---

## How to Run

1. Clone the repository.
2. Install dependencies from requirements.txt.
3. Download the Netflix Prize Dataset.
4. Run Netflix_Recommendation_System.ipynb.

---

## Future Improvements

* Hybrid Recommendation Systems
* Deep Learning Approaches
* Cold Start Handling
* Metadata-Based Recommendations
* Large-Scale Distributed Training
