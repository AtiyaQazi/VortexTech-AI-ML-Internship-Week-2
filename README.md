# VortexTech AI-ML Internship-Week 2

## Machine Learning Classification Model

This project is part of the **VortexTech AI-ML Internship-Week 2**. It demonstrates a complete machine learning classification workflow using the **Titanic dataset** and Scikit-learn.

The project covers data exploration, preprocessing, train-test splitting, classification model training, evaluation using multiple metrics, model comparison, and visualization.

---

## Project Objective

The objective of this project is to build a classification model that predicts whether a passenger **survived or did not survive** based on information available in the Titanic dataset.

The target variable is:

* **Survived**

  * `0` = Did not survive
  * `1` = Survived

Two classification algorithms are trained and compared:

1. Logistic Regression
2. Decision Tree Classifier

---

## Dataset

The project uses the **Titanic passenger dataset**.

The dataset contains information such as:

* Passenger class
* Sex
* Age
* Number of siblings/spouses
* Number of parents/children
* Fare
* Port of embarkation
* Survival status

The target variable used for classification is **Survived**.

---

## Machine Learning Workflow

The notebook follows these steps:

### 1. Data Loading

The Titanic dataset is loaded using Pandas and inspected to understand its structure, columns, data types, and target variable.

### 2. Data Exploration

The dataset is explored to identify:

* Number of observations
* Available features
* Data types
* Missing values
* Target distribution
* Basic statistical information

### 3. Data Preprocessing

The dataset is prepared for machine learning by handling missing values and converting categorical variables into numerical values.

Categorical features such as **Sex** and **Embarked** are converted using `pd.get_dummies()`.

Missing values are handled before model training.

### 4. Feature and Target Selection

The target variable is:

```text
Survived
```

The remaining selected passenger attributes are used as input features.

### 5. Train-Test Split

The dataset is divided into training and testing sets using an **80/20 split**.

```python
train_test_split(
    X,
    y,
    test_size=0.2,
    random_state=42
)
```

The training set is used to train the models, while the testing set is used to evaluate their performance.

### 6. Model Training

Two classification models are trained using Scikit-learn:

* Logistic Regression
* Decision Tree Classifier

### 7. Prediction

After training, both models generate predictions on the unseen test dataset.

### 8. Model Evaluation

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score

### 9. Model Comparison

The performance of both models is compared using a results table and visualization.

---

## Models Used

### Logistic Regression

Logistic Regression is used as the primary classification model because it is a simple and effective algorithm for binary classification problems.

### Decision Tree Classifier

A Decision Tree Classifier is also trained to compare its performance with Logistic Regression.

Using two models provides a simple comparison of different classification approaches on the same dataset.

---

## Evaluation Metrics

The following classification metrics are used:

### Accuracy

Measures the percentage of total predictions that are correct.

### Precision

Measures how many of the passengers predicted as survivors actually survived.

### Recall

Measures how many of the actual survivors were correctly identified.

### F1-Score

Provides a balance between precision and recall.

---

## Results

The models achieved the following results on the test dataset:

| Model               | Accuracy | Precision | Recall | F1-Score |
| ------------------- | -------: | --------: | -----: | -------: |
| Logistic Regression |   81.01% |    78.57% | 74.32% |   76.39% |
| Decision Tree       |   78.21% |    72.73% | 75.68% |   74.17% |

### Best Performing Model

Based on the evaluation results, **Logistic Regression performed better overall**, achieving an accuracy of approximately **81.01%** compared with **78.21%** for the Decision Tree.

The Logistic Regression model also achieved a higher precision and F1-score. The Decision Tree achieved slightly higher recall, meaning it identified a slightly larger proportion of actual survivors.

The models are reasonably effective, but their performance can still be improved through better feature engineering, hyperparameter tuning, and cross-validation.

---

## Technologies Used

* **Python**
* **Jupyter Notebook**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Scikit-learn**

---

## Project Structure

```text
VortexTech-AI-ML-Internship-Week-2/
│
├── data/
│   └── train.csv
│
├── Week2_ML_Classification.ipynb
├── README.md
└── .gitignore
```

The Jupyter Notebook contains the complete machine learning implementation, including:

* Data loading
* Data exploration
* Data preprocessing
* Feature and target preparation
* Train-test splitting
* Model training
* Predictions
* Evaluation metrics
* Model comparison
* Visualization

---

## Installation

Make sure Python is installed on your system.

Install the required libraries using:

```bash
pip install numpy pandas matplotlib scikit-learn jupyter
```

---

## How to Run

### 1. Clone the repository

```bash
git clone https://github.com/AtiyaQazi/VortexTech-AI-ML-Internship-Week-2.git
```

### 2. Navigate to the project directory

```bash
cd VortexTech-AI-ML-Internship-Week-2
```

### 3. Start Jupyter Notebook

```bash
jupyter notebook
```

### 4. Open the notebook

Open the `.ipynb` file and run the cells sequentially from beginning to end.

---

## Reproducibility

The notebook contains the complete workflow required to reproduce the classification experiments.

Running the notebook performs:

1. Data loading
2. Data exploration
3. Data preprocessing
4. Feature and target preparation
5. Train-test splitting
6. Logistic Regression training
7. Decision Tree training
8. Predictions
9. Model evaluation
10. Model comparison
11. Visualization

A fixed `random_state=42` is used for the train-test split to make the experiment reproducible.

---

## Future Improvements

The model could be improved through:

* Hyperparameter tuning
* Cross-validation
* Feature engineering
* Feature selection
* Additional classification algorithms
* Better handling of class imbalance
* More advanced visualization
* Model deployment through an API or web application

---

## Internship

**VortexTech AI-ML Internship-Week 2**

This project demonstrates practical implementation of machine learning classification concepts as part of the VortexTech AI/ML Internship Program 2026.

---

## Author

**Attia Qamar-un-Nisa**

Computer Science Graduate
