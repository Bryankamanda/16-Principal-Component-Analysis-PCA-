
#  Principal Component Analysis (PCA) – Dimensionality Reduction on Digits Dataset

##  Project Overview

This project explores **Principal Component Analysis (PCA)** as a dimensionality reduction technique and evaluates its impact on classification performance using the **Digits dataset**.

The focus is to understand how reducing feature space affects model accuracy while improving computational efficiency.

---

##  Dataset

* **Dataset Used:** Digits Dataset
* **Source:** `sklearn.datasets`
* **Description:**

  * Handwritten digit images (0–9)
  * Each image is represented by **64 features (8×8 pixels)**
* **Target:** Digit classification (0–9)

---

##  Project Workflow

### 1. Data Preparation

* Loaded dataset from `sklearn`
* Split into features (**X**) and target (**y**)
* Applied **feature scaling (Standardization)**

---

### 2. Dimensionality Reduction (PCA)

Applied PCA under three scenarios:

* **100% variance (all 64 components)**
* **95% explained variance**
* **2 principal components**

---

### 3. Model Training

* Trained a classification model on:

  * Original dataset
  * PCA-transformed datasets

---

### 4. Model Evaluation

* Evaluated using **accuracy score**
* Compared performance across different feature dimensions

---

##  Results & Insights

| Scenario           | Features Used | Accuracy   |
| ------------------ | ------------- | ---------- |
| Original Data      | 64 (100%)     | **97.22%** |
| PCA (95% Variance) | Reduced       | **96.95%** |
| PCA (2 Components) | 2             | **60.80%** |

---

##  Key Takeaways

* PCA can reduce dimensionality with **minimal performance loss**
* Retaining **95% variance preserved nearly all predictive power**
* Extreme reduction (2 components) caused **significant information loss**
* Clear trade-off between:

  * Model simplicity & speed
  * Predictive performance

---

##  Tech Stack

* Python 
* Pandas
* NumPy
* Matplotlib / Seaborn
* Scikit-learn

---

##  How to Run

```bash
# Clone the repository
git clone https://github.com/Bryankamanda/16-Principal-Component-Analysis-PCA-.git

# Navigate into the project
cd 16-Principal-Component-Analysis-PCA-

# Launch notebook
jupyter notebook
```

##  Author

**Bryan Kamanda**
Data Science | Analytics | Banking Operations

