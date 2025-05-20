# Sampling Techniques and Model Performance Analysis

This project evaluates the effectiveness of different sampling techniques in handling imbalanced datasets. The dataset contains credit card transactions with imbalanced classes, requiring the application of resampling methods to improve model performance.

## Overview

The task involved:
1. **Balancing the Dataset**: Using various sampling techniques to address class imbalance.
2. **Sampling Techniques Used**:
   - **SMOTE**
   - **Random Under-Sampling**
   - **Random Over-Sampling**
   - **Near Miss**
   - **SMOTEENN**
3. **Machine Learning Models Tested**:
   - **M1**: AdaBoostClassifier
   - **M2**: DecisionTreeClassifier
   - **M3**: ExtraTreesClassifier
   - **M4**: LinearDiscriminantAnalysis
   - **M5**: GaussianProcessClassifier
4. **Performance Metric**: Accuracy was used to evaluate the performance of each model with each sampling technique.

## Results

The table below shows the best sampling technique for each model based on accuracy:

| **Model** | **Best Sampling Technique** | **Accuracy** |
|-----------|-----------------------------|--------------|
| M1        | Sampling5 (SMOTEENN)        | 96.12%       |
| M2        | Sampling1 (SMOTE)           | 95.69%       |
| M3        | Sampling1 (SMOTE)           | 98.71%       |
| M4        | Sampling5 (SMOTEENN)        | 81.47%       |
| M5        | Sampling1 (SMOTE)           | 93.53%       |

## File Descriptions

- **`sampling_results.csv`**: Contains the full accuracy results for all sampling techniques and models.
- **`best_sampling_techniques.csv`**: Highlights the best sampling technique for each model.

## Conclusion

The results demonstrate that **SMOTE** and **SMOTEENN** were the most effective sampling techniques for handling the class imbalance in this dataset. These techniques improved the accuracy of most models significantly.

---

Feel free to use this file or modify it based on additional insights! Let me know if you need further help.
