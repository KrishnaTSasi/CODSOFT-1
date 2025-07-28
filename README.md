# CODSOFT-1

This repository contains my internship tasks for the CODSOFT program.

 ✅ Task 1: Movie Genre Classifier using ML and TF-IDF

In this task, we built a genre classification model using different machine learning algorithms:
- Logistic Regression
- SVM
- Naive Bayes


We used `TF-IDF` to vectorize movie plot summaries and trained models to classify the genre.

🔧 Features used:
- Plot summary (text)
- Genre (target variable)

 📊 ML Models Used:
- Logistic Regression
- SVM
- Naive Bayes

 📊 Model Evaluation – Accuracy Results

We evaluated the performance of different machine learning models on the movie genre classification task using TF-IDF vectorization of plot summaries.

 ⚙️ Accuracy Scores:

| Model                | Accuracy (%) |
|----------------------|--------------|
| Naive Bayes          | 30.1%        |
| Logistic Regression  | 39.8%        |
| Support Vector Machine (SVM) | 40.7%  |

 🧠 Interpretation:

- All three models perform **just above random guessing**, indicating that:
  - The dataset may be **too small** to capture genre-specific patterns.
  - Plot summaries are **short or overlapping in content**, reducing TF-IDF effectiveness.
  - **Genres may overlap** (e.g., Action vs. Thriller), confusing classifiers.
- **SVM performed the best**, suggesting it's slightly more effective at handling the high-dimensional sparse TF-IDF vectors.
- **Naive Bayes performed the worst**, possibly due to strong independence assumptions not holding in short plot texts.


**

### 📁 Files:
- `movie_genre_classifier.ipynb` — Jupyter notebook with complete code
- `genre_sample_data.csv` — Sample dataset with plots and genres

---

## 📦 Requirements

```bash
pip install -r requirements.txt
