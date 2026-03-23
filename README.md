# Lab6_KNN_Classification
"Wine dataset classification using PCA &amp; KNN. Achieved ~96% accuracy before PCA and ~98% after dimensionality reduction, with explained variance highlighting preserved information.


Overview:
This lab explores the impact of Principal Component Analysis (PCA) on classification performance using the Wine dataset.
We apply K-Nearest Neighbors (KNN) before and after PCA to compare accuracy, interpret trade-offs, and analyze explained variance.
The goal is to demonstrate how dimensionality reduction affects model performance and information preservation.


Step 1: Import Libraries:
scikit-learn (datasets, train_test_split, StandardScaler, PCA, KNN, metrics)
numpy, matplotlib, seaborn (optional for visualization)


Load Dataset:
Dataset: Wine dataset from scikit-learn.

Features: Chemical analysis attributes of wines.

Target: Wine class labels (multi-class classification).


Step 3: Split Dataset:
Training set: 70%

Test set: 30%

Random state fixed for reproducibility.

Standardize Data:
StandardScaler applied to ensure fair distance-based comparisons in KNN.


Part A: Before PCA

Train KNN classifier (k=5) on scaled data.
Accuracy BEFORE PCA: 0.9629 (~96.3%)

Part B: Apply PCA

PCA applied with 2 components.
Reduced dimensionality while preserving maximum variance.


Explained Variance Ratio: [0.3619, 0.1876] (≈55% of variance preserved).


Part C: After PCA

Train KNN classifier (k=5) on PCA-transformed data.
Accuracy AFTER PCA: 0.9814 (~98.1%)

Conclusion:
Before PCA: High accuracy demonstrates KNN’s strength with full data.

After PCA: Accuracy slightly improved, showing PCA preserved essential variance while reducing dimensionality.

Explained Variance: PCA retained ~55% of dataset variance, balancing performance and dimensionality reduction.

Overall, PCA not only reduced complexity but also enhanced accuracy, highlighting its value in classification tasks.

