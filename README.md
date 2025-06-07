# AI-ML-Internship-Task7

# 🧠 Heart Disease Classification with SVMs

This project implements Support Vector Machines (SVMs) using both **linear** and **non-linear (RBF)** kernels to classify heart disease presence.

---

## 📌 Objective

Use SVMs for binary classification to predict whether a patient has heart disease based on clinical features.

---

## 🧰 Tools & Libraries

- Python
- NumPy, Pandas
- Scikit-learn
- Matplotlib

---

## 🗂️ Dataset

- **File**: `heart_disease_uci.csv`
- **Source**: UCI Heart Disease Repository
- **Target Column**: `num` (converted to binary as `target`)
- **Rows**: 920
- **Features**: Age, Chest Pain Type, Cholesterol, Max Heart Rate, etc.

---

## 🧪 Steps Performed

| Step | Description |
|------|-------------|
| 1. | Data Cleaning & Encoding |
| 2. | Train-Test Split |
| 3. | Feature Scaling |
| 4. | PCA (for 2D visualization) |
| 5. | SVM with Linear and RBF Kernels |
| 6. | Hyperparameter Tuning using GridSearchCV |
| 7. | Evaluation using Accuracy and Cross-Validation |

---

## 📊 Results

### 🎯 Accuracy Comparison

| Model      | Test Accuracy | Cross-Validation |
|------------|---------------|------------------|
| Linear SVM | 80.87%        | 77.71%           |
| RBF SVM    | 80.87%        | 77.60%           |

### 🔍 Best RBF Parameters

- **C**: 1  
- **Gamma**: 0.1  
- **Best CV Score**: 80.43%

---

## 📈 PCA Visualization

PCA was applied to reduce the data to 2 components for decision boundary visualization. (You can visualize with `plt.scatter(X_pca[:,0], X_pca[:,1], c=y)`).

---

## 🏁 How to Run

1. Upload `heart_disease_uci.csv` to your notebook/Colab.
2. Run the code provided in the notebook/script.
3. Ensure all required Python libraries are installed.
4. Modify hyperparameters for tuning if needed.

---

## 📚 References

- [UCI Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/heart+disease)
- [Scikit-learn SVM Docs](https://scikit-learn.org/stable/modules/svm.html)

