📊 Amazon Product Price Prediction
Advanced Multimodal ML for Price Estimation | Amazon ML Challenge 2025

This repository contains a comprehensive machine learning solution developed to predict product prices using Amazon’s high-dimensional dataset of 75,000 products. By leveraging multimodal feature engineering (Text + Image), we achieved a significant 25–35% reduction in error compared to baseline models.

🚀 Project Overview
Predicting market prices requires understanding both the quantitative attributes of a product and its qualitative appeal. Our approach focuses on a sophisticated feature engineering pipeline that transforms raw multimodal data into a robust 30-feature vector, optimizing for Mean Absolute Error (MAE) and RMSE.

📈 Key Highlights
Feature Engineering: Generated 24–30 engineered features to capture semantic and visual nuances.

Multimodal Fusion: Integrated NLP and Computer Vision pipelines into a unified model architecture.

Optimization: Experimented with ensemble methods (XGBoost/LightGBM) and Custom Neural Networks.

Results: Consistently achieved a 25–35% error reduction over traditional regression benchmarks.

🛠️ Technical Implementation
1. Multimodal Feature Pipeline
To capture the full context of a product, we developed separate but complementary processing tracks:

Textual Analysis (NLP):

Tokenization and embedding generation using semantic analysis.

Feature extraction from product titles, descriptions, and bullet points.

Visual Analysis (CV):

Deep learning embeddings extracted from product images.

Feature engineering based on color histograms, aspect ratios, and object detection.

The Fusion Layer: A specialized concatenation strategy to combine sparse text vectors with dense image embeddings.

2. Model Architecture
We evaluated the performance of three distinct modeling strategies:

Gradient Boosting (XGBoost/LightGBM): Used for its high interpretability and handling of tabular engineered features.

Neural Networks: Custom architectures utilizing dropout and batch normalization to prevent overfitting on the multimodal embeddings.

Ensemble Methods: A weighted average of regression and neural outputs to stabilize predictions.
