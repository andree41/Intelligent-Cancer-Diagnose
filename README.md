# Intelligent Cancer Diagnosis

## Project Overview
This project aims to diagnose breast cancer using machine learning techniques. It leverages a dataset derived from digitized images of fine needle aspirate (FNA) of breast masses to classify tumors as either malignant or benign. The project includes data preprocessing, model selection, hyperparameter tuning, and performance evaluation. Three classifiers—Logistic Regression, Support Vector Machine (SVM), and Random Forest—are implemented and evaluated for their diagnostic accuracy.

## Dataset Overview
The dataset contains features calculated from digitized images of breast masses, capturing various characteristics such as mean radius, texture, perimeter, and area. Each record corresponds to a diagnostic analysis, with the target variable being the diagnosis (malignant or benign). The dataset is available in the file `Assignment3-Breast-Cancer-Diagnose.csv`. 600x33

## Data Preprocessing
- **Binary Conversion**: The 'diagnosis' variable is encoded into binary format (malignant = 1, benign = 0).
- **Handling Missing Values**: Missing values are imputed using the mean of their respective columns.
- **Feature Selection**: Unnecessary features, including the patient ID, are dropped.
- **Normalization**: Feature scaling is recommended, especially for models like SVM.

## Model Selection and Implementation
Three classifiers are selected based on their diverse mechanisms:
- **Logistic Regression**: A fundamental approach providing a probabilistic perspective.
- **Support Vector Machine (SVM)**: Capable of handling nonlinear relationships through the kernel trick.
- **Random Forest**: An ensemble method that improves prediction accuracy and robustness.

## Hyperparameter Tuning
- **Random Forest**: Tuning focused on `n_estimators` and `max_depth`. GridSearchCV was used to find the optimal configuration (`max_depth=10`, `n_estimators=200`).


## Performance Evaluation
- **Logistic Regression**: 95.61%
- **SVM**: 94.74%
- **Random Forest**: 95.61%

## Conclusion and Recommendations
The project demonstrates the feasibility and efficiency of machine learning classifiers in diagnosing breast cancer. The comparable performance of the classifiers highlights the importance of considering multiple models and tuning parameters for such critical applications. The selection of hyperparameters played a pivotal role in enhancing the classifiers' performance, underscoring the importance of a meticulous tuning process in achieving high diagnostic accuracy. Future work could explore additional features, larger datasets, and more advanced models to further improve diagnostic accuracy.
