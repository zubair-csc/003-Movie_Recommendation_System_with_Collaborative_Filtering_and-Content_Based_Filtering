# 🧠 Movie Recommendation System with Collaborative & Content-Based Filtering

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

## 📋 Project Overview
This project implements a **hybrid movie recommendation system** combining **content-based filtering** (using TF-IDF similarity on movie metadata) and **collaborative filtering** (via matrix factorization with SVD). It features a full pipeline: data loading from the MovieLens dataset, model building, evaluation with RMSE & MAE, and personalized movie recommendations.

---

## 🎯 Objectives
- Recommend movies based on user preferences and movie content
- Implement and compare content-based and collaborative filtering
- Evaluate model performance using industry-standard metrics
- Enable dynamic predictions with collaborative filtering
- Visualize similarity, predictions, and results (optional extension)

---

## 📊 Dataset Information
**Dataset**: [MovieLens Latest Small Dataset (100k ratings)](https://grouplens.org/datasets/movielens/)  
**Size**: ~100,000 ratings, ~9,000 movies  
**Files**:
- `movies.csv`: Movie metadata (title, genres)
- `ratings.csv`: User ratings (userId, movieId, rating)

**Target Output**: Top-N movie recommendations  
**Filtering Techniques**:
- **Content-Based**: TF-IDF on genres and titles
- **Collaborative**: User-movie rating matrix with SVD

---

## 🔧 Technical Implementation

### 📌 Recommendation Algorithms
- **Content-Based Filtering**: TF-IDF vectorization + cosine similarity
- **Collaborative Filtering**: Matrix factorization via Surprise’s SVD

### 🧹 Data Preprocessing
- TF-IDF vectorization of movie genres and titles
- Mapping userId ↔ movieId interactions
- Building similarity matrix for efficient lookups

### ⚙️ Modeling
- Train/test split for collaborative filtering
- 3-fold cross-validation for SVD
- Rating predictions for unseen items

### 📏 Evaluation Metrics
- **Collaborative Filtering**: RMSE, MAE
- **Content-Based**: Cosine similarity (unsupervised)

### 📊 Visualizations (Optional)
- Cosine similarity heatmap
- Top-N recommended movies per user
- RMSE/MAE plot across folds

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Google Colab or Jupyter Notebook

### Installation
Clone the repository:
```bash
git clone https://github.com/zubair-csc/003-Movie_Recommendation_System_with_Collaborative_Filtering_and-Content_Based_Filtering.git
cd 003-Movie_Recommendation_System_with_Collaborative_Filtering_and-Content_Based_Filtering
