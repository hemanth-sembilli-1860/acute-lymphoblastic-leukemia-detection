[![IEEE Xplore](https://img.shields.io/badge/IEEE-Published-blue)](https://ieeexplore.ieee.org/document/xxxxxxxx)
# Acute Lymphoblastic Leukemia Detection Using FCM Segmentation + EfficientNetB4 + XGBoost

This project presents a hybrid machine learning pipeline for detecting **Acute Lymphoblastic Leukemia (ALL)** from blood smear images.  
It combines:

- **Fuzzy C-Means (FCM) segmentation**
- **EfficientNetB4 deep feature extraction**
- **GPU-accelerated XGBoost classification**
- **Interpretability via qualitative error analysis**

###🎯 Final Test Accuracy: **95.53%**

---

##📌 1. Dataset
- **Blood Cell Cancer (ALL 4-Class)**  
  https://www.kaggle.com/datasets/mohammadamireshraghi/blood-cell-cancer-all-4class  
- Used only for **research / academic / educational** purposes.

Classes converted into:
- **0 → Benign**
- **1 → Malignant (Early Pre-B, Pre-B, Pro-B)**

---

##📌 2. Pipeline Overview

Raw Image
↓
FCM Segmentation
↓
EfficientNetB4 Feature Extraction
↓
XGBoost Classifier
↓
Benign / Malignant Prediction


---

## 📌 3. Features of the Model

✔ Unsupervised segmentation using Fuzzy C-Means  
✔ Pretrained EfficientNetB4 for robust features  
✔ XGBoost for efficient binary classification  
✔ GPU acceleration  
✔ Training & validation curves  
✔ Confusion matrix + metrics  
✔ TP / FP / TN / FN qualitative visualizations  

---

## 📌 4. How to Run

### Install Dependencies
pip install -r requirements.txt


### Run the Notebook
Open:


segmentation_and_classification.ipynb


All steps are included for segmentation, feature extraction, training, and evaluation.

---

## 📌 5. Results

### ✔ Final Accuracy: **95.53%**

The model prints a detailed classification report including:
- Precision
- Recall
- F1-score
- Support

A qualitative visualization of predictions (TP, FP, FN, TN examples)  
has been saved as:

results/qualitative_analysis.png
results/segmentation_examples/

## 📌 6. File Structure



ALL_Leukemia_Detection_Model/
│
├── results/
│ ├── qualitative_analysis.png
│ └── segmentation_examples/
│
├── src/
│ ├── fcm_segmentation.py
│ ├── feature_extraction.py
│ ├── xgboost_classifier.py
│ └── utils.py
│
├── segmentation_and_classification.ipynb
├── requirements.txt
├── LICENSE
└── README.md


---

## 📌 7. License
Licensed under **MIT License** (see `LICENSE` file).

---

## 📌 8. Disclaimer
This project is for **research and educational purposes only**.  
It is **NOT** a clinical diagnostic tool.

---

## 📌 9. Author
**Tagore**  
Machine Learning Student  
Open to internships & freelance ML work.
