<div align="center">

# 🌸 Iris Flower Classification

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)](https://seaborn.pydata.org)

> **Can a machine learn to distinguish flower species just from measurements?**
> A multiclass classification project using Decision Tree — with full EDA and visualizations.

</div>

---

## 📌 Problem Statement

The Iris dataset contains 150 samples of 3 flower species — **Setosa**, **Versicolor**, and **Virginica** — each described by 4 measurements: sepal length, sepal width, petal length, and petal width. The goal is to build a classifier that accurately predicts the species from these measurements alone.

---

## 🎯 Project Highlights

| What | Detail |
|------|--------|
| 🧠 Algorithm | Decision Tree Classifier |
| 📦 Dataset | Iris dataset — 150 samples, 4 features, 3 classes |
| 🎯 Target | Species — Setosa / Versicolor / Virginica |
| 📊 Key Features | Sepal Length, Sepal Width, Petal Length, Petal Width |
| ✅ Accuracy | ~96% on test set |

---

## 🗂️ Project Structure

```
iris-flower-classification/
│
├── iris_flower_classification.ipynb  # Jupyter Notebook — EDA + model + visualizations
├── requirements.txt                  # Dependencies
├── images/                           # Visualization outputs
└── README.md
```

---

## 🔄 ML Pipeline

```
Load Data  →  EDA  →  Visualization  →  Model Training  →  Evaluation  →  Feature Importance
```

**Step-by-step:**

1. **Load Data** — Iris dataset via Scikit-learn, structured into Pandas DataFrame
2. **EDA** — Feature distributions, class balance, summary statistics
3. **Visualize** — Pairplots and correlation heatmap to understand separability
4. **Train/Test Split** — 80/20 split using `train_test_split`
5. **Train Model** — Decision Tree Classifier
6. **Evaluate** — Accuracy score + Confusion Matrix
7. **Feature Importance** — Which measurement matters most?

---

## 📊 Key Findings

- 🌼 **Setosa** is perfectly linearly separable from the other two species
- 🌿 **Petal length and petal width** are the most powerful features for classification
- 🔀 **Versicolor and Virginica** have some overlap — where most misclassifications happen
- 📐 **Sepal width** alone is the weakest predictor across all three species

---

## 📈 Visualizations

> All charts are available in the `images/` folder and rendered inside the notebook.

- Pairplot — feature relationships across all 3 species
- Correlation heatmap — feature interdependencies
- Confusion matrix — model prediction accuracy per class
- Feature importance bar chart — top contributing measurements

---

## ⚙️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/keerthanad29/iris-flower-classification.git
cd iris-flower-classification

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter Notebook
jupyter notebook iris_flower_classification.ipynb
```

> Or open directly in **Google Colab** — no setup needed!

---

## 📦 Requirements

```
pandas
numpy
scikit-learn
matplotlib
seaborn
```

---

## 🧠 Model Performance

| Metric | Score |
|--------|-------|
| Accuracy | ~96% |
| Classes | Setosa / Versicolor / Virginica |
| Evaluation | Confusion Matrix + Classification Report |

---

## 💡 What I Learned

- How to perform **Exploratory Data Analysis (EDA)** on a multiclass dataset
- Why **pairplots and heatmaps** are essential before model building
- How **Decision Trees** handle non-linear boundaries in multiclass classification
- Reading and interpreting a **confusion matrix** for 3-class problems
- Understanding **feature importance** to explain model decisions

---

## 🔮 Future Improvements

- [ ] Compare Decision Tree vs Random Forest vs KNN
- [ ] Add cross-validation for more reliable accuracy estimate
- [ ] Deploy as a simple web app using Streamlit
- [ ] Experiment with hyperparameter tuning (max_depth, min_samples_split)
