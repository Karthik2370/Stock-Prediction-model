# 📰 Stock Market Headline Predictor

A machine learning project that predicts stock market trends based on financial news headlines.

## 📘 About the Project

This project explores the connection between daily news headlines and stock market movements. By analyzing the language used in financial news, the model attempts to forecast market direction for a given day.

## ⚙️ Features

- Uses historical financial headlines as input
- Applies text preprocessing (punctuation removal, lowercasing)
- Implements Bag of Words model with bi-grams for feature extraction
- Trains a Random Forest Classifier for prediction
- Evaluates performance using accuracy, confusion matrix, and classification report

## 📁 Dataset

The dataset contains:
- `Date` — date of the news
- `Label` — market movement (1 for up, 0 for down)
- `Top1` to `Top25` — 25 news headlines for each day

> Note: The dataset uses `ISO-8859-1` encoding to handle special characters.

## 📈 Model Workflow

1. Split data into training and testing sets based on date
2. Clean and preprocess headlines
3. Combine daily headlines into a single string per day
4. Vectorize text using `CountVectorizer` with bi-grams
5. Train the model using `RandomForestClassifier`
6. Test the model on unseen data
7. Evaluate the results

## 📊 Evaluation Metrics

- **Accuracy Score**
- **Classification Report**
- **Confusion Matrix (Visualized)**

## 📦 Dependencies

- pandas
- scikit-learn
- matplotlib (for visualization, optional)

## 🧠 Goal

To understand how much influence headline sentiment has on short-term stock market direction and whether machine learning can be used effectively to model that relationship.

## 📌 Note

This project is for educational and research purposes only. It is **not** intended for actual stock trading or financial advice.
