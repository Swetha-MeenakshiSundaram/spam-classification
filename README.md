# 📧 SMS Spam Classification using Multinomial Naive Bayes

This project implements a **Spam/Ham SMS classification model** using the **Multinomial Naive Bayes algorithm** and **TF-IDF vectorization**.  
The dataset used is the **SMS Spam Collection Dataset**, which contains labeled SMS messages as either **ham** (not spam) or **spam**.

---

## 📂 Dataset
- **Source**: https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset/data
- **Size**: 5,574 SMS messages
- **Labels**:
  - `ham` → Non-spam messages
  - `spam` → Unwanted/spam messages

---

## 🛠 Preprocessing Steps
1. **Lowercasing** – Convert all text to lowercase for uniformity.
2. **Removing punctuation** – Eliminate special characters and symbols.
3. **Stopword removal** – Remove common words (e.g., "the", "and") using NLTK stopword list.
4. **TF-IDF Vectorization** – Convert text into numerical features using **Term Frequency–Inverse Document Frequency**.

---

## 🤖 Model Used
- **Multinomial Naive Bayes (MultinomialNB)** from `scikit-learn`
- Chosen because it works well for **text classification** with discrete word counts or TF-IDF features.

---

## 📊 Results

| Metric  | Training Score | Testing Score |
|---------|---------------|---------------|
| Accuracy | 97.78%        | 96.77%        |

**Classification Report:**

<img width="507" height="432" alt="image" src="https://github.com/user-attachments/assets/47b7f980-a4f1-45e8-9ecc-8b6e6c9625a0" />

