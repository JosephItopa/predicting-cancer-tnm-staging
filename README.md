## SMM4H-HeaRD 2026: Predicting TNM Staging from TCGA Pathology Reports

This paper describes the procedure, methods, and results on the classification of TNM staging based on the extracted pathology reports. Our approach leverages conventional machine learning and deep learning approaches: (1) Logistic Regression, (2) Light Gradient-boost, and (3) Wide Residual Neural network.

## 1. Data

The data use in this research is the data provided by the competition organizer, which can be accessed through the data folder in this repo.


## 2. System Architecture

### 2.1 Overview

Our system architecture implements an TF-IDF and Auto-encoder based classification pipeline with three core components:

1. **Data Preprocessing:** Feature Engineering, and encoding
2. **TNM Classification:** TNM classification using machine learning and deep learning.
3. **Evaluation:** Performance evaluation of the models.

### 2.2 Project Data
The project data can be found through the README on the data folder of this repo. The data is stored in CSV files and it contained fields such as: patient file name, text, T, N, and M.


### 2.3 Folder Structure

#### ├── data/
#### │   └── model_hyperparameter_settings.csv
#### │
#### ├── dl_notebook/
#### │   ├── data_preprocessing_and_encoding_v4.ipynb
#### │   ├── deep_learning_bert_modelling_wrnM.ipynb
#### │   ├── deep_learning_bert_modelling_wrnN.ipynb
#### │   └── deep_learning_bert_modelling_wrnT.ipynb
#### │
#### ├── ml_notebook/
#### │   ├── ML_NLP_imbalanced.ipynb
#### │   └── ML_NLP_smote.ipynb
#### │
#### ├── src/
#### │
#### └── README.md

## 3. How to run the code

1. The notebook for machine learning can be run locally, but the notebooks for deep learning reuirees GPU. Therefore, Google Colab is recommended.  
2. The libraries can be installed via a cell on the notebook or you can install on a virtual environment through: pip install -r requirements.txt 
3. The hyperparameter settings can be found on the CSV file in the data folder of this repo.

