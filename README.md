[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://colab.research.google.com/github/KiarashMafi/Classification-Projects/blob/main/Random%20Forest%20Classifier/random_forest_classifier.ipynb
)

# Classification Models Comparison

This project demonstrates the implementation and visualization of different machine learning classification models, including:

- **Random Forest Classifier**
- **Kernel SVM**
- **K-Nearest Neighbors (K-NN)**
- **Decision Tree Classifier**

## Dataset

We use **Social_Network_Ads.csv** (`400` rows, `3` columns). The likely target/label is **`Purchased`**.
Features used for modeling come from these columns:
  - `Age`
  - `EstimatedSalary`


**Class distribution** (`Purchased`): 0: 257, 1: 143.

**Numeric feature summary:**  
- **Age** — min: 18.0, mean: 37.66, max: 60.0
- **EstimatedSalary** — min: 15000.0, mean: 69742.5, max: 150000.0

> Notes
> - In typical versions of this dataset, models are trained on `Age` and `EstimatedSalary` to produce the 2D decision regions shown below.
> - If you change features, update the plotting code accordingly.

## Project Overview

The notebooks included in this repository show how to preprocess, train, evaluate, and visualize these classifiers on the dataset.
Each notebook corresponds to a different classification algorithm and plots the learned decision boundary on the test set.

### Preprocessing (common steps)

- Split the dataset into **training** and **test** sets.
- Apply **standardization** to numeric features for distance/kernel-based models (K-NN, SVM).
- Fit the model on the training set, then evaluate/plot on the test set.

## Result on Test Set

The following figure shows the decision boundaries of all four models on the test set:


<img width="3000" height="3000" alt="Untitled design" src="https://github.com/user-attachments/assets/bfb268cb-c803-428d-afab-1556da253976" />

## Files Included

- `random_forest_classifier.ipynb` — Random Forest.
- `kernel_svm.ipynb` — Kernel SVM.
- `knn.ipynb` — K-Nearest Neighbors.
- `decision_tree_classifier.ipynb` — Decision Tree.
- `Social_Network_Ads.csv` — Dataset used.
- `Untitled design.png` — Visualization of the results on the test set.

## How to Run

1. Open any of the notebooks in Jupyter.
2. Ensure `Social_Network_Ads.csv` is in the same directory (or update the path).
3. Run all cells to train and visualize the classifiers.
