# Classifying Emails as Spam or Not Spam

**Project by:** Syeda Umaima Tamkeen

## 📝 Summary

In this project, I developed a classification model to automatically detect whether an email is **spam** or **not spam**, using a dataset of labeled emails. I implemented both **Naive Bayes** and **Support Vector Machine (SVM)** classifiers, achieving **100% accuracy** on both. This solution demonstrates an efficient spam detection system that can enhance user experience and reduce unsolicited communications.

---

## 🔍 Key Steps

### 1. Data Exploration
- Analyzed patterns in the email dataset.
- Visualized the distribution of spam vs. non-spam to understand class balance.

### 2. Data Preprocessing
- Cleaned the dataset by:
  - Removing punctuation, digits, and stopwords.
  - Handling missing values.
- Applied **stemming** to reduce words to their root form.
- **Tokenized** and **vectorized** text using **TF-IDF**, keeping the top 3000 most informative features.

### 3. Feature Extraction
- Used **TF-IDF vectorization** to convert text data into numerical format.
- Captured key terms that distinguish spam from non-spam.

### 4. Model Training
- Trained and evaluated two models:
  - **Multinomial Naive Bayes**
  - **Support Vector Machine (SVM)** with linear kernel
- Used **train-test split** for validation.

### 5. Model Evaluation
Both models achieved **perfect accuracy** on the dataset:
- **Naive Bayes Accuracy:** 1.00
- **SVM Accuracy:** 1.00

Evaluation metrics confirmed perfect:
- **Precision**
- **Recall**
- **F1-Score**

### 6. Model Fine-Tuning
Used **GridSearchCV** to optimize parameters:
- **Naive Bayes:** `alpha = 0.5`
- **SVM:** `C = 0.1`, `kernel = 'linear'`

These optimizations further refined performance while maintaining accuracy.

---

## ✅ Results

**Final Model Performance:**

| Model        | Accuracy | Precision | Recall | F1-Score |
|--------------|----------|-----------|--------|----------|
| Naive Bayes  | 1.00     | 1.00      | 1.00   | 1.00     |
| SVM (Linear) | 1.00     | 1.00      | 1.00   | 1.00     |

**Best Hyperparameters:**
- **Naive Bayes:** `alpha = 0.5`
- **SVM:** `C = 0.1`, `kernel = 'linear'`

---

## 📌 Conclusion

Both **Naive Bayes** and **SVM** models performed exceptionally well in classifying emails as spam or not spam, achieving **100% accuracy** on the dataset. While this result is promising, future work could:
- Test on **larger, real-world datasets**
- Handle **class imbalance**
- Explore **ensemble techniques** for robustness

This project demonstrates the potential of machine learning to create powerful spam detection systems suitable for real-world deployment.

