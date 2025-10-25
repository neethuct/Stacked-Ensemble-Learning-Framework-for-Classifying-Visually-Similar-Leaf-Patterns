# **Project Title**
**A Stacked Ensemble Learning Framework for Classifying Visually Similar Leaf Patterns of Popular Indian *Hevea* Clones Using Shape Descriptive Features**

---

## **Project Description**
This project presents an AI-based framework for the automated classification of visually similar Indian *Hevea* (rubber plant) clones — RRII 105, RRII 414, RRII 417, RRII 422, and RRII 430.  
The approach uses shape-descriptive leaf features and applies **Dynamic Time Warping (DTW)** to capture subtle border variations.  
A stacked ensemble of **SVM**, **XGBoost**, and **DNN** classifiers is employed, achieving an **accuracy of 82%** in clone identification.

---

## **Dataset**
│Data
├── Training.csv # 28 feature columns + 1 'label' column (clone name)
├── Test.csv # Similar structure as Training.csv

---

## **Software Platform and Packages Used**

- **Programming Language:** Python 3.9+  
- **Development Environment:** Google Colab / Jupyter Notebook  

### **Key Libraries**
- **NumPy** — numerical computations  
- **Pandas** — data handling and preprocessing  
- **Scikit-learn** — machine learning models and metrics  
- **TensorFlow / Keras** — deep learning (DNN) implementation  
- **XGBoost** — gradient boosting model  
- **Optuna** — hyperparameter optimization  
- **Matplotlib** — plotting and visualization  
- **Seaborn** — advanced data visualization  
- **SHAP** — interpretability analysis  
- **Pickle / Joblib** — model saving and loading  

---

## **How to Run**
1. Open the project in **Google Colab** or **Jupyter Notebook**.  
2. Upload the training and testing CSV files.  
3. Execute all cells in the provided notebook (`Dataset_PLN2EnsembleOptunaVF.ipynb`).  
4. The notebook will automatically train models, evaluate accuracy, and display confusion matrix and performance metrics.  

---

## **Result**
- Final stacked ensemble model achieved **82% classification accuracy** in distinguishing visually similar *Hevea* clones.  
- Feature interpretability was analyzed using **SHAP** to identify the most influential leaf shape descriptors.

---

## **License**
This repository is for **academic and research use only**.
