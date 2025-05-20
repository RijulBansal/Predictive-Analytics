# 🔍 SVM Parameter Optimization on a Multi-Class Dataset

This project focuses on optimizing the hyperparameters of a Support Vector Machine (SVM) classifier using a multi-class dataset, as part of a machine learning assignment.

---

## 📁 Project Structure

---

## 📘 Overview

**Objectives:**
- Choose a multi-class dataset containing 5,000–30,000 samples.
- Apply SVM classification and tune its `kernel`, `C`, and `gamma` parameters.
- Evaluate performance on **10 different random samples** from the dataset.
- Run **100 iterations** with various parameter combinations.
- Report the best accuracy and parameter set for each sample.
- Plot a **convergence graph** showing accuracy versus iterations.

---

## 🧠 Key Concepts

- Support Vector Machine (SVM)
- Hyperparameter Tuning
- Data Augmentation with Gaussian Noise
- Accuracy Evaluation
- Visualization with Matplotlib
- Scikit-learn’s SVC, `train_test_split`, and `StandardScaler`

---

## 📊 Dataset

- **Source:** `sklearn.datasets.load_wine()`
- **Classes:** 3 (multi-class)
- **Expansion:** The dataset was synthetically increased to **5,000 samples** using Gaussian noise.

---

## 🛠️ Requirements

Install the following dependencies:

```bash
pip install numpy pandas scikit-learn matplotlib
```

## ⚙️ Methodology

1. **Data Preparation:**
   - Load the Wine dataset and expand it to 5,000 samples by adding Gaussian noise.
   - Standardize features using `StandardScaler`.

2. **Sampling Strategy:**
   - Generate 10 random samples using different random seeds.
   - Split each sample into 80% training and 20% testing sets.

3. **SVM Optimization Loop:**
   - For each sample, train an SVM classifier 100 times with different combinations of:
     - C (Regularization): [0.1, 1, 10, 100]
     - gamma (Kernel coefficient): ['scale', 0.01, 0.1, 1]
     - kernel: ['linear', 'rbf']

4. **Evaluation:**
   - Calculate accuracy for each configuration.
   - Record the best-performing configuration for each sample.

5. **Performance Analysis:**
   - Plot accuracy scores from all iterations to visualize convergence.
   - Store the best parameters and accuracies in a results table.

## 📈 Sample Results Table

![image](https://github.com/user-attachments/assets/811193bd-6dda-45d5-a830-ecbb06aba364)

## 📉 Convergence Graph

The convergence graph displays accuracy scores across iterations for each of the 10 samples, illustrating how model performance changes with different parameter sets and whether accuracy stabilizes as more configurations are tested.

- **X-axis:** Iteration number (1 to 100)
- **Y-axis:** Accuracy
- **Lines:** One per sample

This visualization helps determine:
- If further tuning could improve performance
- Which samples consistently perform better
- The stability of the model