# 📧 Spam Classifier Web App

A machine learning-based web application that classifies SMS messages as **Spam** or **Not Spam** using Natural Language Processing (NLP) and a trained ML model.

### 🚀 Deployed App
Check it out live 👉 [https://spamclassifier-7hq4.onrender.com](https://spamclassifier-7hq4.onrender.com)

---

## 📌 Features

- Clean and modern UI built with Bootstrap
- NLP-based text preprocessing (tokenization, stopword removal, stemming)
- TF-IDF vectorization
- Trained classification model (e.g., Naive Bayes)
- Flask-based web backend
- Hosted on Render

---

## 🧠 Tech Stack

- Python
- Flask
- Scikit-learn
- NLTK
- HTML/CSS + Bootstrap
- Render (for deployment)

---

                    ┌────────────────────────────┐
                    │      Web Browser (User)    │
                    │  - Enters SMS message      │
                    │  - Clicks Predict button   │
                    └────────────┬───────────────┘
                                 │
                                 ▼
                    ┌────────────────────────────┐
                    │      Flask Web Server      │
                    │   Routes: / and /predict   │
                    └────────────┬───────────────┘
                                 │
               ┌─────────────────┴──────────────┐
               │                                │
               ▼                                ▼
               
   ┌──────────────────────┐        ┌────────────────────────┐
   │ Text Preprocessing   │        │  Load ML Model + TF-IDF│
   │ - Lowercase          │        │  - model.pkl           │
   │ - Tokenization       │        │  - vectorizer.pkl      │
   │ - Stopword Removal   │        └────────────┬───────────┘
   │ - Stemming           │                     │
   └──────────────────────┘                     ▼
                                ┌────────────────────────┐
                                │  Prediction (Spam/Ham) │
                                └────────────┬───────────┘
                                             ▼
                            ┌────────────────────────────────┐
                            │ Rendered back on index.html    │
                            │ Display: "Spam" or "Not Spam"  │
                            └────────────────────────────────┘

---
Thank You

