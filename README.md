# student-performance-prediction-bkt
# Bayesian Knowledge Tracing (BKT)

This project implements a complete Bayesian Knowledge Tracing (BKT) pipeline using Python and the pyBKT library.

The goal of the project is to model student learning behavior and predict future student performance using educational datasets.

The implementation includes preprocessing, chronological interaction ordering, grouped train/test splitting, model training, prediction generation, ROC analysis, Precision-Recall analysis, and evaluation visualizations.

---

# Features

* Educational data preprocessing
* Missing value removal
* Filtering valid student responses
* Removal of multi-skill interactions
* Chronological sorting of interactions
* Group-based train/test splitting
* Bayesian Knowledge Tracing (BKT) training
* ROC Curve visualization
* Precision-Recall Curve visualization
* Confusion Matrix visualization
* Classification metrics evaluation

---

# Technologies

* Python
* pyBKT
* pandas
* NumPy
* scikit-learn
* matplotlib

---

# Data Preprocessing

The preprocessing pipeline includes:

* Selecting only required columns
* Removing missing values
* Keeping only:

  * `correct`
  * `incorrect`
* Removing rows containing multiple skills (`~~`)
* Sorting student interactions chronologically
* Converting labels:

  * `correct → 1`
  * `incorrect → 0`

---

# Train/Test Split

The dataset is split using:

```python
GroupShuffleSplit
```

This prevents the same student from appearing in both training and testing datasets.

---

# Evaluation Metrics

The implementation evaluates the model using:

* Accuracy
* ROC AUC
* Precision
* Recall
* F1-score
* Confusion Matrix

---

# Visualizations

The project generates:

* ROC Curves
* Precision-Recall Curves
* Confusion Matrix heatmaps

---

# Example Results

## Physics Dataset

* Accuracy: 0.852
* ROC AUC: 0.8933

These results show that the BKT model successfully captures student learning behavior and predicts future responses with strong performance.

---

# Project Structure

```text
analysis/
    scripts/
        bkt_model.py

data/
    raw/

BKT.ipynb
requirements.txt
```

---

# Installation

Install the required packages:

```bash
pip install -r requirements.txt
```

---

# Run

Open and run the notebook:

```text
BKT.ipynb
```

---

# Author

Abdullah Jalab
University of Duisburg-Essen
