# 🧠 Plagiarism Detection using Support Vector Machine (SVM)

## 📌 Project Description
This project builds a machine learning system that detects whether a given text is plagiarized by comparing it with an original source. It uses Natural Language Processing (NLP) techniques and a Support Vector Machine (SVM) classifier for optimal accuracy.

Developed as part of an internship project at **Gwing Software Solutions**.

---

## 📊 Dataset
The dataset used for this project is named **`customer_data.csv`**.

It contains:
- `source_text`: The original content
- `plagiarized_text`: Text that may or may not be plagiarized
- `label`: 
  - `1` → Plagiarism detected
  - `0` → No plagiarism

Total entries: **370**

---

## 🔁 Project Workflow

1. **Install & Import Dependencies**  
   Libraries include NLTK, Scikit-learn, Pandas, Pickle

2. **Load Dataset**  
   Upload and read `customer_data.csv` into a pandas DataFrame

3. **Preprocess Text**  
   - Lowercase text  
   - Remove punctuation  
   - Remove stopwords

4. **Vectorize Text**  
   Use `TfidfVectorizer` to convert text to numeric features

5. **Split Dataset**  
   Use 80/20 stratified split for training/testing

6. **Train Multiple Models**  
   - Logistic Regression  
   - Random Forest  
   - Naive Bayes  
   - **Support Vector Machine (Best Model)**

7. **Evaluate Performance**  
   Metrics: Accuracy, Precision, Recall, F1-score, Confusion Matrix

8. **Save Model & Vectorizer**  
   Store SVM model and TF-IDF vectorizer using `pickle`

9. **Predict on New Text**  
   Provide real-time predictions using a custom detection function

---

## ✅ Model Results

| Model               | Accuracy |
|---------------------|----------|
| Logistic Regression | 82.43%   |
| Random Forest       | 79.73%   |
| Naive Bayes         | 86.48%   |
| **SVM (Best)**      | **87.83%** |

---
