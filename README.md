# 🌸 Iris Flower Classification

## 📌 Project Overview

This project uses machine learning classification techniques to identify the species of an Iris flower based on its physical measurements.

The three Iris species are:

- Setosa
- Versicolor
- Virginica

The project demonstrates a complete machine learning workflow, including data exploration, visualization, feature analysis, model training, evaluation, and model comparison.

## 🎯 Objective

To build and evaluate machine learning classification models that can accurately predict the species of an Iris flower using:

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## 📊 Dataset

The Iris dataset is obtained directly from `sklearn.datasets.load_iris()`.

The dataset contains:

- 150 observations
- 4 numerical features
- 3 Iris species
- 50 samples per species

## 🔍 Exploratory Data Analysis

The following analyses were performed:

- Dataset shape inspection
- Data type inspection
- Missing-value check
- Descriptive statistics
- Species distribution analysis
- Pairplot visualization
- Box plots for all features

The dataset is balanced, with 50 observations for each species.

## 🌸 Feature Selection

Exploratory analysis showed that **petal length and petal width** are the most discriminative features for distinguishing the Iris species.

Random Forest feature importance confirmed this observation:

| Feature | Importance |
|---|---:|
| Petal Width | 0.437185 |
| Petal Length | 0.431466 |
| Sepal Length | 0.116349 |
| Sepal Width | 0.015000 |

Petal width and petal length together contribute approximately **86.87%** of the total feature importance.

## 🤖 Machine Learning Models

Two classification algorithms were trained:

1. Logistic Regression
2. Random Forest Classifier

The dataset was divided into:

- 80% training data
- 20% testing data

A stratified split was used to preserve the class distribution.

## 📈 Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

### Model Performance

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| **Logistic Regression** | **96.67%** | **96.97%** | **96.67%** | **96.66%** |
| Random Forest | 90.00% | 90.24% | 90.00% | 89.97% |

## 🏆 Best-Performing Model

**Logistic Regression** was selected as the best-performing model.

It achieved:

- **96.67% Accuracy**
- **96.97% Precision**
- **96.67% Recall**
- **96.66% F1-Score**

It outperformed Random Forest across all four evaluation metrics on the test dataset.

## 📷 Project Visualizations

### Species Distribution

![Species Distribution](screenshots/01_Species_Distribution.png)

### Pairplot

![Pairplot](screenshots/02_Pairplot.png)

### Feature Box Plots

![Box Plots](screenshots/03_Boxplots.png)

### Logistic Regression Confusion Matrix

![Logistic Regression Confusion Matrix](screenshots/04_Logistic_Confusion_Matrix.png)

### Random Forest Confusion Matrix

![Random Forest Confusion Matrix](screenshots/05_RandomForest_Confusion_Matrix.png)

### Model Comparison

![Model Comparison](screenshots/06_Model_Comparison.png)

### Feature Importance

![Feature Importance](screenshots/07_Feature_Importance.png)

## 📝 Conclusion

The project successfully demonstrated the use of machine learning classification techniques for Iris species prediction.

Exploratory analysis and feature importance showed that **petal length and petal width are the strongest predictors** of Iris species.

Among the two tested models, **Logistic Regression performed best**, achieving an accuracy of **96.67%**.

This project demonstrates a complete and practical machine learning workflow from data exploration to model evaluation and interpretation.

## 📁 Project Structure

```text
OIBSIP-Task1-IrisClassification/
│
├── Iris_Classification.ipynb
├── README.md
└── screenshots/
    ├── 01_Species_Distribution.png
    ├── 02_Pairplot.png
    ├── 03_Boxplots.png
    ├── 04_Logistic_Confusion_Matrix.png
    ├── 05_RandomForest_Confusion_Matrix.png
    ├── 06_Model_Comparison.png
    └── 07_Feature_Importance.png