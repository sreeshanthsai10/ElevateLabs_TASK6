# ElevateLabs_TASK6
# Iris Species Classification with K-Nearest Neighbors (KNN)

This repository contains my solution for **Task 6: K-Nearest Neighbors Classification** from the Elevate AI & ML Internship Labs. The objective was to use KNN to classify Iris flower species using a provided dataset.

---

## What I Did

### 1. **Loaded and Preprocessed Data**
- Used the classic `Iris.csv` dataset containing measurements and labeled species.
- Extracted feature columns and target labels.
- Scaled features using StandardScaler for optimal KNN performance.

### 2. **Split Data**
- Divided the dataset into train and test sets, maintaining class distribution.

### 3. **Built and Evaluated KNN Model**
- Trained KNN classifier using scikit-learn's `KNeighborsClassifier`.
- Experimented with different values of `K` (1–15) and plotted accuracy for each.
- Selected **K=9** (best accuracy: **0.96**).

### 4. **Reported Metrics**
- **Confusion Matrix:**
    ```
    [[15  0  0]
     [ 0 15  0]
     [ 0  2 13]]
    ```
- **Classification Report:**
    - Setosa and Versicolor were classified perfectly.
    - Minor overlap between Versicolor and Virginica.
- **Test Accuracy:** 0.96

### 5. **Visualized Decision Boundaries**
- Plotted KNN decision regions using two features for intuitive illustration.

---

## Key Insights

- **KNN performed extremely well on this dataset**, achieving 96% accuracy.
- **Perfect precision/recall for Setosa and Versicolor**; small misclassification between Virginica and Versicolor due to feature space overlap.
- Feature scaling is **essential** for distance-based algorithms like KNN.

---

## How to Run

1. Clone/download the repo and ensure `Iris.csv` is present.
2. Install requirements:
    ```
    pip install pandas numpy matplotlib scikit-learn
    ```
3. Run `knn_iris.py` to reproduce results, plots, and metrics.

---


