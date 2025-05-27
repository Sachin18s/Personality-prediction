# Personality-prediction
# 🧠 Personality Prediction using MBTI and NLP

This project predicts a user's personality type (MBTI) based on the text they have written. It uses NLP (Natural Language Processing) and Logistic Regression to classify the personality type into four traits:  
- Introvert (I) / Extrovert (E)  
- Intuitive (N) / Sensing (S)  
- Thinking (T) / Feeling (F)  
- Judging (J) / Perceiving (P)

---

## 📁 Dataset

The dataset used is mbti_1.csv, which contains:
- posts: Social media posts written by users.
- type: The MBTI personality type of each user (like INFP, ESTJ, etc.).

Dataset source: [Kaggle - MBTI 5000](https://www.kaggle.com/datasnaek/mbti-type)

---

## ⚙ Technologies and Libraries Used

- Python  
- Pandas  
- Scikit-learn  
- TF-IDF Vectorizer  
- Logistic Regression  
- Regular Expressions (for text cleaning)

---

## 🧹 Text Preprocessing

The text is cleaned using the following steps:
- Lowercasing the text  
- Removing URLs  
- Removing special characters and numbers  
- Keeping only alphabets and spaces

---

## 🧠 Model Training

- The MBTI type is split into 4 binary labels (IE, NS, TF, JP).
- TF-IDF is used to convert text into numeric features.
- Logistic Regression is used to build a model for each personality trait.
- Models are evaluated using classification reports.

---

## 🧪 Example Prediction

```python
sample = "I love to spend time reading books, thinking about ideas, and staying alone."
predicted_type = predict_mbti(sample)
print("Predicted MBTI type:", predicted_type)
