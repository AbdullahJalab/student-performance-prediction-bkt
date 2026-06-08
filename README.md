# Student Performance Prediction

This repository contains implementations of educational data mining models for predicting student performance and learning outcomes using educational datasets.

Currently implemented models:

* Bayesian Knowledge Tracing (BKT)
* Additive Factors Model (AFM)

The project includes data preprocessing, model training, evaluation, and visualization pipelines for comparing different student performance prediction approaches.

---

# Models

## Bayesian Knowledge Tracing (BKT)

BKT models student knowledge as a hidden state that evolves over time.

Features:

* Student-skill sequence modeling
* Knowledge state estimation
* Probability of correct response prediction
* ROC and Precision-Recall evaluation

## Additive Factors Model (AFM)

AFM is a logistic regression-based educational data mining model.

Features:

* Knowledge Component (KC) encoding
* Opportunity count modeling
* Student error prediction
* ROC and Precision-Recall evaluation

---

# Technologies

* Python
* pyBKT
* pandas
* NumPy
* scikit-learn
* matplotlib

---

# Evaluation Metrics

The models are evaluated using:

* Accuracy
* ROC AUC
* Precision
* Recall
* F1-score
* Confusion Matrix

---

# Visualizations

* ROC Curves
* Precision-Recall Curves
* Confusion Matrices

---

# Repository Structure

```text
AFM.ipynb
BKT.ipynb
README.md
requirements.txt
```

---

# Installation

```bash
pip install -r requirements.txt
```

---

# Usage

Run the notebooks individually:

```bash
AFM.ipynb
```

or

```bash
BKT.ipynb
```

---

# Author

Abdullah Jalab

University of Duisburg-Essen
