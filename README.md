# Amazon Reviews Analysis


---


## 💡 Overview

This project implements a complete e-commerce data analysis and machine learning pipeline using a subset of the Amazon Product Dataset. The goal is to extract meaningful insights from product reviews and metadata and apply various machine learning techniques for clustering, classification, recommendation, and sentiment analysis.

The analysis focuses on five selected product categories to demonstrate a comprehensive, end-to-end data science workflow.


---


## 📂 Contents
- **`amazonreviewss.ipynb`** – Initial exploration and preprocessing of Amazon reviews dataset. Includes text cleaning, visualization, and sentiment distribution.
- **`amazonreviews_part2.ipynb`** – Extended analysis with feature extraction, model training (e.g., sentiment classification), and evaluation.


---


## ⚙️ Features

The project is divided into two major parts: Data Pre-processing/Feature Engineering (Part 1) and Machine Learning Tasks (Part 2).

### Part 1: Data Preparation & Feature Engineering

- Data Acquisition & Preparation:
  - Data extracted from JSON format and transformed into CSV files for five chosen categories.
  - Leveraged the Hugging Face datasets library for data loading and filtering.
  - Data cleaning included handling missing values and normalizing prices.
- Exploratory Data Analysis (EDA):
  - Visualized product ratings distribution and average rating trends over time using Matplotlib/Seaborn/Plotly.
  - Identified best-selling products (highest review count) and analyzed their key attributes.
  - Identified outlier products with high review volume but low ratings, analyzing common review keywords.
- Advanced Feature Engineering:
  - Sentiment Feature Engineering: Developed a final sentiment score using a combination of text sentiment (VADER/Hugging Face models) and user ratings. Two
    alternative methods were explored:
    - Weighted Combination: Blending VADER/Hugging Face text sentiment (normalized -1 to +1) with the user rating (normalized 0 to 1) via a weighted average.
    - Rating-Adjusted Sentiment: Amplifying/decreasing text sentiment based on high (4 or 5 stars) or low (1 or 2 stars) numerical ratings.
- Price and Rating Metrics (Optional): Created derived features like Price-per-Feature and a Weighted Rating (adjusted by log(Review Count)) to mitigate rating bias.

### Part 2: Machine Learning Tasks

- Clustering for Product Grouping: Applied clustering techniques (e.g., K-Means) to group similar products based on features, descriptions, and ratings.
  - Involved text cleaning (stemming, lowercasing) and numerical feature scaling.
  - Used Vectorization (e.g., TF-IDF or Word2Vec) on product text descriptions.
- Classification: (A standard part of the assignment, though details are in the second part document not fully provided here). Likely involved classifying sentiment or predicting product success.
- Recommendation System: (A standard part of the assignment). Likely involved user-item matrix analysis or collaborative filtering.
- Sentiment Analysis: Applying models (e.g., those from Scikit-learn or leveraging Hugging Face) to classify review sentiment, building upon the engineered features.


---


## 🧰 Technologies Used & Libraries
- **Language**: Python 3.x  
- **Framework**: Jupyter Notebook  
- **Data Manipulation**: pandas, numpy
- **Data Acquisition**: datasets (Hugging Face) 
- **Sentiment Analysis**: nltk, transformers (Hugging Face) 
- **Visualization**: matplotlib, seaborn 
- **Text Pre-processing**: nltk  
- **ML models & evaluation**: scikit-learn

---


## 📂 Project Structure

├── notebooks/      # Includes the 2 notebooks for the project  
└── README.md       # Project documentation
