# Breast Cancer Classification using Machine Learning

## Overview
This project uses machine learning to classify breast tumours as **Benign (non-cancerous)** or **Malignant (cancerous)** using the Breast Cancer Wisconsin Diagnostic dataset.

Eight classification algorithms are implemented and compared to evaluate their performance on a binary classification task.

## Dataset
The project uses the Breast Cancer Wisconsin Diagnostic dataset.

- **Samples:** 569
- **Features:** 30 numerical features
- **Target:** Diagnosis (Benign or Malignant)
- **Class distribution:** 357 Benign and 212 Malignant samples

The features describe characteristics of cell nuclei, including radius, texture, perimeter, area, smoothness and concavity.

## Algorithms Implemented
- Logistic Regression
- Support Vector Machine (SVM with RBF kernel)
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Gaussian Naive Bayes
- Gradient Boosting
- Extra Trees Classifier

## Technologies Used
- Python
- Pandas and NumPy
- Scikit-learn
- Matplotlib and Seaborn
- Google Colab / Jupyter Notebook

## Workflow
1. Load and explore the dataset.
2. Convert diagnosis labels into binary values (Benign = 0, Malignant = 1).
3. Separate input features from the target variable.
4. Split the data into training (80%) and testing (20%) sets.
5. Apply feature scaling where required using Scikit-learn pipelines.
6. Train and evaluate eight machine learning algorithms.
7. Compare model performance using evaluation metrics and visualisations.

## Evaluation Metrics
The models are evaluated using:

- **Accuracy:** Overall proportion of correct predictions.
- **Precision:** Proportion of predicted malignant cases that are actually malignant.
- **Sensitivity (Recall):** Proportion of actual malignant cases correctly identified.
- **Specificity:** Proportion of actual benign cases correctly identified.
- **F1-Score:** Balance between precision and recall.
- **ROC-AUC:** Ability of a model to distinguish between the two classes.

## Results
Using an 80:20 train-test split, the best results from the current experiment were:

| Metric | Best Performing Model | Score |
|---|---|---:|
| Accuracy | SVM (RBF) | 97.37% |
| Sensitivity | SVM (RBF) | 92.86% |
| ROC-AUC | Extra Trees | 99.87% |

The results demonstrate how different algorithms can perform differently depending on the evaluation metric.

## Visualisations
The notebook includes:
- Confusion matrices for all eight models.
- A comparison chart of model evaluation metrics.
- Classification reports for individual algorithms.

## How to Run
1. Open the notebook in Google Colab or Jupyter Notebook.
2. Install the required libraries if they are not already available.
3. Run the notebook cells.
4. Upload the `breast-cancer.csv` dataset when prompted.
5. Execute the cells sequentially to train and evaluate the models.

## Project Context
Developed alongside my undergraduate Machine Learning coursework to gain practical experience with classification algorithms and model evaluation.

## Disclaimer
This is an educational machine learning project and is not a clinically validated diagnostic tool. Its predictions should not be used for medical diagnosis.
