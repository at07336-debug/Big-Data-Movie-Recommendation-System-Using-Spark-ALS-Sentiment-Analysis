# 🎬 Big Data Movie Recommendation System

### **Spark ALS + Sentiment Analysis | MovieLens 20M + TMDB Metadata**

This project implements a **hybrid movie recommendation system** using **Apache Spark**, combining collaborative filtering with sentiment scoring to generate personalized, context-aware movie recommendations. It uses the **MovieLens 20M** dataset for large-scale user ratings and **TMDB metadata** to compute sentiment scores, producing recommendations that reflect both user preferences and public opinion.

---

## 🚀 Features

* **Big Data Processing with Spark**
  Handles millions of ratings using Spark DataFrames and SQL.

* **Collaborative Filtering (ALS)**
  Trains a scalable model using Spark’s Alternating Least Squares algorithm.

* **Sentiment Integration**
  Converts TMDB movie scores into a normalized sentiment metric (0–1).

* **Hybrid Recommendation Logic**
  Combines predicted ALS rating + sentiment score for more reliable suggestions.

* **Netflix-Style Popup UI (Colab)**
  A lightweight interactive popup that displays:
  ✔ Predicted rating
  ✔ Sentiment score
  ✔ Recommendation decision
  ✔ Similar movies

* **Analytics & Reports**
  Includes sentiment distribution, genre trends, rating–sentiment comparison, and top recommendations.

---

## 📦 Datasets Used

### **MovieLens 20M Dataset**

* 20M user ratings
* 27K movies
* Source: GroupLens Research

### **TMDB Metadata**

* Genres, release year, popularity
* Score-based sentiment
* Used for movie-level context

---

## 🧠 Project Workflow

1. **Load datasets** using Spark & KaggleHub
2. **Clean & normalize titles** (remove punctuation, parentheses)
3. **Compute sentiment** from TMDB scores
4. **Join datasets** using Spark SQL
5. **Train ALS model** on millions of user–movie ratings
6. **Predict user-specific ratings** for any movie
7. **Combine ALS + sentiment** for final recommendation
8. **Display results** in a popup UI built with ipywidgets

---

## 📊 Reports Generated

* Top 10 recommendations (ALS)
* Sentiment distribution histogram
* Genre-wise sentiment analysis
* Rating vs sentiment comparison
* Similar movie suggestions

---

## 🖥️ How to Run

1. Open the notebook in **Google Colab**
2. Install dependencies (Spark, KaggleHub)
3. Upload your `kaggle.json`
4. Run all cells to:

   * Download datasets
   * Build the Spark pipeline
   * Train the ALS model
   * Launch the popup UI

---

## 🔧 Technologies Used

* Python
* Apache Spark / PySpark
* KaggleHub API
* Pandas / Matplotlib
* ipywidgets
* Google Colab

---

## 📝 Repository Description (Short)

*A Spark-based hybrid movie recommender using MovieLens 20M and TMDB metadata. The system trains an ALS model, integrates sentiment, and provides real-time recommendations through a Netflix-style popup UI.*

---

## 📚 References (APA)

GroupLens. (2015). *MovieLens 20M Dataset*.
Zhou, Y., Wilkinson, D., Schreiber, R., & Pan, R. (2008). *Large-scale collaborative filtering*.
Apache Spark Documentation. (2024).
TMDB Metadata Dataset (Kaggle).

---
