# Arch-Technologies_Iris-Flower-Classification
Month 2, Task 4

This project implements **Task 4: Iris Flower Classification** from the Arch Technologies Machine Learning internship assignment.

The objective is to build a machine learning classification model that predicts the species of an Iris flower from its measured physical characteristics. The project is implemented in a Jupyter Notebook and covers data loading, inspection, preprocessing, model training, evaluation, confusion-matrix analysis, and feature-importance visualization.

---

## **Project Objective**

The goal of this project is to develop a classification model capable of predicting the Iris flower species from its input measurements.

The workflow includes:

* Loading the Iris dataset
* Inspecting the dataset structure
* Checking missing values
* Checking class distribution
* Separating features and target
* Performing a stratified train-test split
* Handling missing values
* Training a Random Forest classifier
* Evaluating the model using accuracy, precision, recall, and F1-score
* Generating a confusion matrix
* Analyzing feature importance
* Visualizing feature importance

---

## **Dataset**

The project uses the **Iris dataset (`IRIS.csv`)** supplied for the Arch Technologies internship task.

### **Target Variable**

`species`

### **Input Features**

* `sepal_length`
* `sepal_width`
* `petal_length`
* `petal_width`

---

## **Machine Learning Approach**

### **1. Data Preprocessing**

The four numerical measurements are used as input features, while `species` is used as the target variable.

Missing numerical values are handled using **median imputation**.

The preprocessing and model are implemented using a Scikit-learn `Pipeline`.

### **2. Train/Test Split**

The dataset is divided using an **80/20 stratified train-test split** with:

```text
random_state = 42
```

Stratification helps preserve the class distribution in both training and testing sets.

### **3. Model**

The project uses:

**Random Forest Classifier**

Configuration:

```text
n_estimators = 180
random_state = 42
n_jobs = -1
```

Random Forest was selected because it can model non-linear relationships and also provides feature-importance information.

---

## **Model Evaluation**

The classifier is evaluated using:

### **Accuracy**

Measures the proportion of correctly classified samples.

### **Precision**

Measures the proportion of positive predictions that are correct.

### **Recall**

Measures how many samples belonging to a class were correctly identified.

### **F1-Score**

Combines precision and recall into a single evaluation metric.

A complete **classification report** is also generated in the notebook.

---

## **Confusion Matrix**

The notebook generates a confusion matrix to provide a class-by-class view of the predictions.

It helps identify:

* Correctly classified samples
* Misclassified samples
* Class-level prediction performance

---

## **Feature Importance**

The Random Forest feature-importance values are extracted and visualized to show the relative contribution of:

* Sepal length
* Sepal width
* Petal length
* Petal width
---

## **Installation**

Clone the repository:

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd Iris-Flower-Classification
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

Activate it on macOS/Linux:

```bash
source venv/bin/activate
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

---
## **Author**

**Affan Abdullah**
**Computer Science**

**Machine Learning Intern**
**Arch Technologies**

