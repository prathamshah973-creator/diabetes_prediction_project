# Diabetes Prediction using KNN Classification

## Project Overview

This project focuses on data cleaning, statistical analysis, visualization, and machine learning classification using a diabetes dataset. The main goal of the project is to understand how patient symptoms and demographic information can be used to predict whether a person is likely to be diabetic or non-diabetic.

The project was completed as part of my Artificial Intelligence and Machine Learning coursework. Through this project, I learned how to handle real-world style data, clean missing values, analyze features, visualize patterns, and build a basic machine learning model using the K-Nearest Neighbors algorithm.

> Note: This project is created for academic learning purposes only. It is not intended to be used as a real medical diagnosis system.

---

## Dataset Information

The dataset used in this project is the **Early Stage Diabetes Risk Prediction Dataset**.

It contains:

- 520 patient records
- 17 columns
- 16 input features
- 1 target column

### Main Features

The dataset includes patient information such as:

- Age
- Gender
- Polyuria
- Polydipsia
- Sudden weight loss
- Weakness
- Polyphagia
- Genital thrush
- Visual blurring
- Itching
- Irritability
- Delayed healing
- Partial paresis
- Muscle stiffness
- Alopecia
- Obesity

### Target Variable

The target column is:

- `class`

It contains two possible values:

- Positive
- Negative

---

## Objectives of the Project

The main objectives of this project were:

1. To understand the structure and characteristics of the diabetes dataset.
2. To perform data cleaning and missing value handling.
3. To carry out statistical analysis of numerical and categorical features.
4. To visualize important patterns in the dataset.
5. To encode categorical variables for machine learning.
6. To apply feature scaling before using KNN.
7. To train and evaluate a K-Nearest Neighbors classification model.
8. To understand the role of preprocessing in machine learning performance.

---

## Technologies Used

- Python
- pandas
- NumPy
- Matplotlib
- scikit-learn
- Jupyter Notebook / Google Colab

---

## Project Workflow

### 1. Data Loading

The dataset was loaded using pandas. The first step was to inspect the dataset shape, columns, data types, and missing values.

### 2. Data Cleaning

The original dataset did not contain missing values. However, artificial missing values were introduced for academic demonstration of data cleaning techniques.

Missing values were handled using:

- Mean imputation for numerical data
- Mode imputation for categorical data

After cleaning, the dataset had no missing values remaining.

### 3. Statistical Analysis

Statistical analysis was performed to understand the dataset better. Since `Age` is the main numerical feature, descriptive statistics such as mean, median, mode, standard deviation, minimum, maximum, range, and variance were calculated.

Categorical columns were analyzed using unique value counts and frequency counts.

### 4. Data Visualization

Several visualizations were created using Matplotlib, including:

- Scatter plot of Age vs Class
- Line graph showing age trend
- Histogram of age distribution
- Bar chart showing missing values after cleaning

These visualizations helped in understanding the distribution of patient age and the cleanliness of the dataset after preprocessing.

### 5. Encoding

Since most features were categorical, they were converted into numerical form.

Examples:

- Yes → 1
- No → 0
- Male → 1
- Female → 0
- Positive → 1
- Negative → 0

### 6. Feature Scaling

Feature scaling was performed using StandardScaler. This step is important for KNN because KNN is a distance-based algorithm, and features with larger values can otherwise dominate the distance calculation.

### 7. Model Training

The dataset was split into:

- 80% training data
- 20% testing data

A K-Nearest Neighbors classifier was trained using:

```python
KNeighborsClassifier(n_neighbors=5)
**###8. Model Evaluation**

The model was evaluated using:

Accuracy
Precision
Recall
F1 Score

The model achieved strong performance on the test set.

###9. Model Perfomance
| Metric    | Score |

| Accuracy  | 93.3% |
| Precision | 98.3% |
| Recall    | 90.6% |
| F1 Score  | 94.3% |
###10. Key learnings
Key Learnings

Through this project, I learned:

How to load and inspect a dataset using pandas.
How to handle missing values using imputation.
How to analyze numerical and categorical features.
How to visualize data using Matplotlib.
Why categorical encoding is necessary before machine learning.
Why feature scaling is important for distance-based algorithms like KNN.
How to train and evaluate a basic classification model.
How model performance should be judged using multiple metrics, not only accuracy.

###11.Limitations
This project has some limitations:

The dataset is relatively small.
The model was trained only on one dataset.
KNN was the main algorithm used.
The project is for academic purposes and cannot be used for real medical diagnosis.
Further validation on larger and more diverse datasets would be required before any practical use.
