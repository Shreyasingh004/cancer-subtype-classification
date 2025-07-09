# cancer-subtype-classification
ML-based classification of cancer subtypes from gene expression data using PCA/UMAP, XGBoost, and SHAP."
# 🧬 Cancer Subtype Classification from Gene Expression Data

This project applies machine learning to classify cancer subtypes based on gene expression profiles. It uses dimensionality reduction techniques (PCA/UMAP), machine learning models (Random Forest/XGBoost), and SHAP for model interpretability. A Streamlit dashboard is used to visualize predictions and feature importance.

---

## 📌 Objective

Classify cancer subtypes using gene expression datasets (e.g., TCGA, GEO) and interpret the important genes contributing to each classification.

---

## 🛠️ Tools & Technologies

- **Python**
- **scikit-learn**
- **XGBoost**
- **UMAP / PCA**
- **SHAP (SHapley Additive exPlanations)**
- **Streamlit**

---

## 📂 Dataset Sources

- **TCGA (The Cancer Genome Atlas):**  
  https://portal.gdc.cancer.gov/

- **GEO (Gene Expression Omnibus) Example:**  
  https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE45827

---

## 📊 Project Workflow

1. **Download gene expression profiles** from TCGA or GEO.
2. **Preprocess the data** (filter, normalize, encode labels).
3. **Apply PCA or UMAP** for dimensionality reduction.
4. **Train classifiers** (Random Forest / XGBoost).
5. **Interpret the model** using SHAP for gene importance.
6. **Build a Streamlit dashboard** to display predictions and visualizations.

---

## 🗃️ Repository Structure
cancer-subtype-classification/
│
├── data/ # Raw and processed data
│ └── README.md # Data download instructions
│
├── notebooks/ # Jupyter notebooks for each step
│ ├── 01_data_exploration.ipynb
│ ├── 02_dimensionality_reduction.ipynb
│ ├── 03_model_training.ipynb
│ └── 04_shap_analysis.ipynb
│
├── src/ # Modular Python scripts
│ ├── preprocessing.py
│ ├── model.py
│ └── visualization.py
│
├── dashboard/ # Streamlit app
│ └── app.py
│
├── requirements.txt # Project dependencies
├── README.md # Project documentation
└── .gitignore
