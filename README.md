# 📧 Spam Classifier Web App

A machine learning-based web application that classifies SMS messages as **Spam** or **Not Spam** using Natural Language Processing (NLP) techniques and a trained ML model.

---

## 🚀 Live Demo

🔗 **Deployed on Render**:  
👉 [https://spamclassifier-7hq4.onrender.com](https://spamclassifier-7hq4.onrender.com)

---

## 🧰 Tech Stack

- **Frontend**: HTML, CSS, Bootstrap
- **Backend**: Python, Flask
- **Machine Learning**: Scikit-learn, NLTK
- **Deployment**: Render

---

## 🎯 Features

- 🔍 Real-time prediction of SMS messages as Spam or Not Spam
- 🧠 Uses trained ML model with TF-IDF vectorization
- ✨ Clean UI built with Bootstrap
- ☁️ Hosted and accessible via Render

---

## 📐 High-Level Design (HLD)

```plaintext
Frontend (HTML/CSS + Bootstrap)
Deployed via Render

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
 │   Text Preprocessing │        │  Load ML Model + TF-IDF│
 │  - Lowercase         │        │  - model.pkl           │
 │  - Tokenization      │        │  - vectorizer.pkl      │
 │  - Stopword Removal  │        └────────────┬───────────┘
 │  - Stemming          │                     │
 └──────────────────────┘                     ▼
                                ┌────────────────────────┐
                                │  Prediction (Spam/Ham) │
                                └────────────┬───────────┘
                                             ▼
                            ┌────────────────────────────────┐
                            │ Rendered back on index.html    │
                            │ Display: "Spam" or "Not Spam"  │
                            └────────────────────────────────┘
