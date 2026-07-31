# Road Traffic Accident Injury & Patient Status Prediction using Machine Learning

## Project Overview

Road traffic accidents (RTAs) are a major public health concern worldwide, causing significant injuries and fatalities every year. Accurate prediction of patient status and injury type following a road traffic accident can support timely medical intervention, improve emergency response, and assist healthcare resource allocation.

This project presents a comparative machine learning study using the **Road Traffic Accident Dataset (Rawalpindi, Punjab, Pakistan)** to predict two important outcomes:

- Patient Status
- Injury Type

Multiple machine learning algorithms were trained, evaluated, and compared to identify the most effective models for each prediction task.

---

# Objectives

The project consists of two independent classification problems:

### 1. Patient Status Prediction

Predict the patient's status after a road traffic accident using multiple supervised machine learning algorithms.

Notebook:

```
notebooks/01_Patient_Status_Prediction.ipynb
```

---

### 2. Injury Type Prediction

Predict the type of injury sustained by a patient using the same dataset and preprocessing pipeline.

Notebook:

```
notebooks/02_Injury_Type_Prediction.ipynb
```

---

# Dataset

**Dataset:** Road Traffic Accident Dataset (Rawalpindi, Punjab, Pakistan)

Dataset Statistics

- Records: **46,189**
- Features: **25**

The dataset is publicly available and is therefore **not included** in this repository.

Please place the downloaded Excel file inside:

```
data/
└── RTA Data 2020 to July 2023.xlsx
```

---

# Data Preprocessing

The following preprocessing techniques were applied before model training:

- Handling missing values
- Duplicate removal
- Outlier detection
- Label Encoding for categorical variables
- Train-test split (80:20)

Three different feature scaling techniques were evaluated:

- StandardScaler
- MinMaxScaler
- RobustScaler

---

# Machine Learning Models

The following supervised classification algorithms were implemented and compared:

- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- XGBoost
- Artificial Neural Network (ANN)

Each model was evaluated under different preprocessing and feature scaling strategies.

---

# Evaluation Metrics

Model performance was assessed using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Classification Report

---

# Results

The comparative evaluation demonstrated that:

### Injury Type Prediction

- Logistic Regression achieved consistently strong performance.
- Artificial Neural Networks (ANN) also produced high prediction accuracy.

### Patient Status Prediction

- Decision Tree performed strongly for patient status classification.
- Random Forest achieved competitive and reliable results.

These findings demonstrate the potential of machine learning techniques to assist road traffic accident analysis and support healthcare decision-making.

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- TensorFlow / Keras
- Jupyter Notebook

---

# Project Structure

```
road-traffic-accident-injury-prediction/
│
├── data/
├── notebooks/
│   ├── 01_Patient_Status_Prediction.ipynb
│   └── 02_Injury_Type_Prediction.ipynb
├── report/
├── images/
├── README.md
├── requirements.txt
├── .gitignore
└── COPYRIGHT.md
```

---

# How to Run

1. Clone this repository.
2. Install the required Python packages.

```bash
pip install -r requirements.txt
```

3. Download the dataset and place it inside the `data/` folder.
4. Open either notebook depending on the prediction task.

---

# Future Improvements

Potential future enhancements include:

- Hyperparameter optimization
- Cross-validation
- Explainable AI (SHAP/LIME)
- Feature importance analysis
- Model deployment using Flask or FastAPI
- Docker containerization
- CI/CD pipeline
- End-to-end MLOps workflow

---

# Author

**Sumaiya Islam Putul**

This repository contains an academic machine learning project developed for educational and portfolio purposes.

© 2026 Sumaiya Islam. All rights reserved.