# Logistic Regression Classification Workflow using Orange

This repository contains a data mining and machine learning workflow built using **Orange Data Mining**. The project demonstrates how to load a dataset, select specific features, train a **Logistic Regression** model, and evaluate its performance.

## 📌 Workflow Overview

The diagram below shows the complete visual programming pipeline designed in Orange:

<p align="center">
  <img src="workflow.png" alt="Orange Data Mining Workflow" width="80%">
</p>

### Workflow Components (Widgets)
1. **File:** Loads the initial dataset into the workspace.
2. **Select Columns:** Filters and designates which features are independent variables (features) and which one is the target variable (class).
3. **Logistic Regression:** A supervised learning algorithm used to predict categorical outcomes.
4. **Test and Score:** Evaluates the model's performance using metrics like AUC, Classification Accuracy (CA), F1-score, Precision, and Recall.

---

## ⚙️ Data Flow & Connections

* **File ➔ Select Columns:** Passes the raw loaded data to the feature selection step.
* **Select Columns ➔ Test and Score:** Sends the processed evaluation data/test set directly for testing.
* **Select Columns ➔ Logistic Regression:** Passes the training data to feed and train the machine learning model.
* **Logistic Regression ➔ Test and Score:** Passes the trained "Learner" object to be evaluated.

---

## 📊 Expected Results

When you double-click on the **Test and Score** widget in this workflow, it opens an evaluation panel showing the model's performance metrics:

<p align="center">
  <img src="results.png" alt="Test and Score Results Evaluation" width="70%">
</p>

| Model | AUC | Classification Accuracy (CA) | F1 Score | Precision | Recall |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Logistic Regression** | *Value* | *Value* | *Value* | *Value* | *Value* |

---

## 🚀 How to Run this Project

1. Download and install [Orange Data Mining](https://orangedatamining.com/).
2. Clone or download this repository.
3. Open the `.ows` (Orange Workflow) file included in this repo.
4. Make sure the **File** widget points to your dataset file, and press refresh if necessary.
