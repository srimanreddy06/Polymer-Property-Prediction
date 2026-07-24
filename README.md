# 🧪 Polymer Property Prediction using Machine Learning

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10-blue?logo=python">
  <img src="https://img.shields.io/badge/RDKit-Cheminformatics-green">
  <img src="https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange">
  <img src="https://img.shields.io/badge/Kaggle-AISEHack%202.0-20BEFF?logo=kaggle">
  <img src="https://img.shields.io/badge/License-MIT-red">
</p>

---

# 📌 Overview

This project was developed for the **ANRF AISEHack 2.0 – Polymer Property Prediction** Kaggle Competition.

The objective is to predict important polymer properties directly from their **SMILES (Simplified Molecular Input Line Entry System)** representation using **Machine Learning** and **Cheminformatics**.

Instead of performing expensive laboratory experiments, researchers can estimate polymer properties computationally, reducing research time and accelerating the discovery of sustainable materials.

---

# 🎯 Problem Statement

Develop a machine learning model capable of predicting two important polymer properties:

- **Glass Transition Temperature (Tg)**
- **Chain Band Gap (Egc)**

using only the polymer's **SMILES** representation.

The competition evaluates predictions using the **Mean R² Score** across both target properties.

---

# 🌍 Why This Project?

Traditional polymer discovery requires:

- Laboratory synthesis
- Material characterization
- Thermal testing
- Electrical measurements

These experiments are:

- Expensive
- Time-consuming
- Resource-intensive

Machine Learning enables researchers to screen thousands of polymers before laboratory testing, significantly reducing cost and development time.

---

# 💡 Objectives

- Predict Tg accurately
- Predict Egc accurately
- Build a complete machine learning pipeline
- Generate a Kaggle-compatible submission file
- Demonstrate the use of AI in materials science

---

# 📂 Dataset

## Training Dataset

| Column | Description |
|---------|-------------|
| smiles | Polymer SMILES representation |
| target | Property value |
| target_type | Tg or Egc |

**Training Samples:** 6171

---

## Test Dataset

| Column | Description |
|---------|-------------|
| id | Unique identifier |
| smiles | Polymer structure |
| target_type | Tg or Egc |

**Test Samples:** 4115

---

# 🔬 About SMILES

SMILES (Simplified Molecular Input Line Entry System) is a text-based representation of molecular structures.

Example:

```text
CC(C)CCCCC=C
```

RDKit converts these molecular structures into numerical descriptors that machine learning algorithms can process.

---

# ⚙️ Project Workflow

```text
            Polymer SMILES
                  │
                  ▼
      RDKit Feature Extraction
                  │
                  ▼
      Molecular Descriptors
                  │
                  ▼
      Feature Engineering
                  │
                  ▼
      Machine Learning Model
                  │
                  ▼
        Tg & Egc Prediction
                  │
                  ▼
          submission.csv
```

---

# 🏗️ Technology Stack

## Programming Language

- Python

## Libraries

- Pandas
- NumPy
- RDKit
- Scikit-learn
- Matplotlib

## Development Environment

- Kaggle Notebook
- Jupyter Notebook

---

# 🧠 Machine Learning Pipeline

### Step 1

Load the datasets.

### Step 2

Convert SMILES into molecular descriptors using RDKit.

### Step 3

Perform feature engineering.

### Step 4

Train a regression model.

### Step 5

Evaluate the model using the Mean R² metric.

### Step 6

Predict polymer properties.

### Step 7

Generate a Kaggle-compatible submission file.

---

# 📊 Evaluation Metric

The competition uses the average coefficient of determination (R²):

```
Score = (R²(Tg) + R²(Egc)) / 2
```

Higher scores indicate better predictive performance.

---

# 🚀 Features

- Polymer Property Prediction
- Molecular Descriptor Generation
- SMILES Processing
- Machine Learning Regression
- Kaggle Submission Generation

---

# 🌎 Applications

- Sustainable Polymer Research
- Biomedical Materials
- Flexible Electronics
- Battery Technology
- Aerospace Engineering
- Automotive Materials
- Eco-friendly Packaging

---

# 📁 Repository Structure

```text
Polymer-Property-Prediction/
│
├── README.md
├── notebook.ipynb
├── requirements.txt
├── .gitignore
├── LICENSE
├── Polymer_Property_Prediction_Detailed_Report.pdf
└── images/
```

---

# ▶️ Installation

Clone the repository:

```bash
git clone https://github.com/srimanreddy06/Polymer-Property-Prediction.git
```

Move into the project directory:

```bash
cd Polymer-Property-Prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

---

# 📈 Results

- Successfully trained a machine learning model.
- Predicted Tg and Egc values for unseen polymers.
- Generated a valid Kaggle `submission.csv`.
- Demonstrated the application of AI in materials science.

---

# 🔮 Future Improvements

- LightGBM
- CatBoost
- XGBoost
- Graph Neural Networks (GNNs)
- ChemBERTa
- Hyperparameter Optimization
- Ensemble Learning

---

# 👨‍💻 Author

**Sriman Narayana Reddy**

- GitHub: https://github.com/srimanreddy06

---

# 📜 License

This project is licensed under the MIT License.

---

⭐ If you found this project useful, consider giving it a star on GitHub!
