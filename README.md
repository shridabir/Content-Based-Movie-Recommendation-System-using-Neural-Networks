# Content-Based-Movie-Recommendation-System-using-Neural-Networks
This project implements a **content-based recommender system** using a **neural network** to predict movie preferences based on user interests and movie features.

## 🧩 Project Overview

The goal of this project is to recommend movies to users by analyzing the **content attributes** (e.g., genres, features, keywords) of movies they've previously rated highly.

Unlike collaborative filtering, which relies on other users’ preferences, **content-based filtering** uses only the current user’s past ratings and the characteristics of movies.

---

## 🧠 Key Steps

### 1️⃣ Packages
- Load required libraries for data processing, visualization, and model building.

### 2️⃣ Dataset
- Load and preprocess the movie ratings dataset.
- Handle missing values, normalize features, and encode categorical data.

### 3️⃣ Content-Based Filtering
- Construct feature vectors for movies and users.
- Combine these into training examples for the neural network.

### 4️⃣ Neural Network Model
- Implement a simple **feedforward neural network** using TensorFlow/Keras.
- Input: movie content features.
- Output: predicted rating (user’s preference score).
- Train the model using Mean Squared Error (MSE) loss.

### 5️⃣ Predictions
- Generate recommendations for:
  - **New users** (cold start via profile building)
  - **Existing users**
- Identify **similar movies** using cosine similarity on learned embeddings.

### 6️⃣ Results
- Evaluate model performance.
- Display sample recommendations and similarity scores.

---

## 🧰 Requirements

Install dependencies using:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow
```

## 🚀 How to Run
- Clone this repository: git clone https://github.com/yourusername/content-based-recommender.git
- Navigate to the project directory: cd content-based-recommender
- Run the notebook or Python script: jupyter notebook content_based_recommender.ipynb
