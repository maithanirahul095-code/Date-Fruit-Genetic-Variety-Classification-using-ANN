# Date Fruit Variety Classification using PyTorch ANN

This project implements an **Artificial Neural Network (ANN)** to classify seven different types of date fruits based on their genetic and morphological features. Using **PyTorch**, the model achieves high accuracy by analyzing 34 distinct image-extracted features.

## 📌 Project Overview
The dataset contains features extracted from images of 898 date fruits belonging to 7 different varieties. The goal is to automate the identification process, which is traditionally done manually by experts.

### Target Classes (7 Varieties):
* Barhee
* Deglet Nour
* Sukkary
* Rotab Mozafati
* Ruthana
* Safawi
* Sagai

### Feature Categories:
The model processes **34 features**, including:
* **Morphological Features:** Area, Perimeter, Major/Minor Axis Length.
* **Shape Features:** Eccentricity, Solidity, Extent.
* **Color Features:** Mean and Standard Deviation of RGB, HSV, and Lab color spaces.

## 🛠️ Technical Stack
* **Language:** Python 3.x
* **Deep Learning:** PyTorch
* **Data Manipulation:** Pandas, NumPy
* **Preprocessing:** Scikit-Learn (`StandardScaler`, `LabelEncoder`)

## 🏗️ Model Architecture
The ANN is a Multi-Layer Perceptron (MLP) designed for multiclass classification:

1.  **Input Layer:** 34 neurons (matching the feature count).
2.  **Hidden Layer 1:** 64 neurons with **ReLU** activation.
3.  **Hidden Layer 2:** 64 neurons with **ReLU** activation.
4.  **Output Layer:** 7 neurons (representing each date variety).

### Training Configuration:
* **Loss Function:** `CrossEntropyLoss` (Ideal for multiclass tasks).
* **Optimizer:** `Adam` (Adaptive Moment Estimation).
* **Epochs:** 100.
* **Batch Size:** 32.

## 📊 Performance Metrics
The model performance is measured by its ability to correctly predict the variety on a held-out test set (20% of the data).

* **Final Accuracy:** [Insert your accuracy here, e.g., 91.5%]
* **Preprocessing:** All features were standardized to a mean of 0 and variance of 1 to ensure stable training.

