# 🛠️ Predictive Maintenance – Machine Learning Project

Predictive maintenance study based on an industrial dataset that includes technical measurements from machines (rotation, torque, temperature, tool wear…) and a failure indicator.  
The goal is to predict whether a machine will fail by using Machine Learning models.

---

## 🎯 Project Objective

Build a model capable of **predicting machine failure (machine failure = 1)** based on its technical parameters.  
The notebook includes:

- Exploratory Data Analysis (EDA)
- Data cleaning and preprocessing
- Machine Learning pipeline construction
- Training several classification models:
  - Logistic Regression  
  - Random Forest  
  - KNN  
  - XGBoost  
- Performance evaluation (classification report + confusion matrix)
- Saving the final trained model

---
## 🔍 Exploratory Data Analysis (EDA)

The notebook starts by exploring the dataset through:

- Dataset inspection  
- Descriptive statistics  
- Correlation analysis  
- Visualizing relationships between features  
- Understanding the main variables:
  - **Rotational speed**  
  - **Torque**  
  - **Tool wear**  
  - **Temperature (air/process)**  
  - **Machine type**  
  - **Machine failure**

Visualizations using **Matplotlib** and **Seaborn** highlight:
- sensor value distributions  
- feature dependencies  
- separation between healthy vs failing machines  

---

## 🧼 Data Preparation & Preprocessing

The notebook performs:

- Feature/target separation  
- Train/test split  
- Encoding of categorical variables  
- Normalization/standardization (depending on the model)

---

## 🤖 Machine Learning Models

The following models are trained:

- **Logistic Regression**
- **Random Forest**
- **K-Nearest Neighbors**
- **XGBoost Classifier**
- **One-vs-Rest classifier** (if needed)

The notebook also includes:

- individual model training  
- model comparison  
- confusion matrix via `ConfusionMatrixDisplay`  
- detailed metrics via `classification_report`

---

## 📊 Model Evaluation

Each model is evaluated using:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**
- **Confusion matrix**

The best-performing model can be saved using:
joblib.dump(model, "best_model.joblib")
