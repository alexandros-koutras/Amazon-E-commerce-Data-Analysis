# Amazon-E-commerce-Data-Analysis


---


## 💡 Overview

This project implements a complete e-commerce data analysis and machine learning pipeline using a subset of the Amazon Product Dataset. The goal is to extract meaningful insights from product reviews and metadata and apply various machine learning techniques for clustering, classification, recommendation, and sentiment analysis.


---


## 📂 Contents
- **`amazonreviewss.ipynb`** – Initial exploration and preprocessing of Amazon reviews dataset. Includes text cleaning, visualization, and sentiment distribution.
- **`amazonreviews_part2.ipynb`** – Extended analysis with feature extraction, model training (e.g., sentiment classification), and evaluation.


---


## ⚙️ Features

The project is divided into two major parts: Data Pre-processing/Feature Engineering (Part 1) and Machine Learning Tasks (Part 2).

### Part 1: Data Preparation & Feature Engineering

- **Data Acquisition & Filtering**:	Loaded and filtered the Amazon Product Dataset using the Hugging Face datasets library to select five specific product categories for feasibility.
- **Pre-processing**:	Data cleaning steps included handling missing values and normalizing price, title, and brand columns.
- **Exploratory Data Analysis (EDA)**: Detailed visualization of product ratings distribution and analysis of review count per product to identify outliers and best-sellers.
- **Sentiment Feature Engineering**: Engineered a final feature, combined_score, using a custom sentiment metric. This metric combines a pre-trained Hugging Face sentiment model's confidence with the normalized
  numerical user rating (normalized 0 to 1).
- **Text Preparation**:	Pre-processed review text using techniques like stop-word removal and lemmatization/stemming in preparation for text-based clustering.

### Part 2: Machine Learning Tasks

- **Clustering for Product Grouping**: Applied the K-Means algorithm on product features and vectorized text data.
- **Classification (Sentiment Prediction)**:	Implemented Classification models (e.g., Logistic Regression, Naive Bayes, Decision Trees) to predict a discrete target variable
- **Model Evaluation**: Thorough evaluation of classification models using metrics: Accuracy, Precision, Recall, and F1-Score.
- **Association Rule Mining**: Apriori Algorithm applied to product transactions to discover frequent itemsets (products often bought together) and generate association rules.


---


## 🧰 Technologies Used & Libraries
- **Language**: Python 3.x  
- **Framework**: Jupyter Notebook  
- **Data Manipulation**: pandas, numpy
- **Data Acquisition**: datasets (Hugging Face) 
- **Sentiment Analysis**: nltk, transformers (Hugging Face) 
- **Visualization**: matplotlib, seaborn 
- **Text Pre-processing**: nltk  
- **ML models**: scikit-learn

---


## 📂 Project Structure

├── notebooks/      # Includes the 2 notebooks for the project  
└── README.md       # Project documentation
