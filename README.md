# 🌿 Plant Disease Detection – ML-based Analysis

This project presents a **machine learning pipeline** for detecting plant diseases using environmental factors like temperature, humidity, rainfall, and soil pH. The work includes data preprocessing, multiple model implementations, performance evaluations, and meaningful visualizations.

It aims to assist in early identification of plant disease risk and support smarter agricultural decision-making.

---

## 📁 Project Structure

This repo contains **3 notebook variants**, each with a different data-handling strategy:

1. **Plant_disease_cleaned_model.ipynb**  
   → Model built after handling null values via cleaning (e.g., mean/mode replacement)

2. **Plant_disease_flagged_model.ipynb**  
   → Model uses null-value flagging to preserve missing data context

3. **Plant_disease_replaced_model.ipynb**  
   → Model after replacing missing values using advanced techniques

All three notebooks are trained and tested using the same core dataset:  
📄 `plant_disease_dataset_merged3.xlsx`

---

## 📌 Dataset Description

| Column           | Description                         |
|------------------|-------------------------------------|
| `temperature`    | Ambient temperature in °C           |
| `Humidity`       | Relative humidity (%)               |
| `rainfall`       | Amount of rainfall in mm            |
| `soil_pH`        | Soil pH value                       |
| `disease_present`| Binary label (1 = Disease present, 0 = Healthy) |

The dataset may contain **missing values**—each notebook addresses these differently.

---

## 🚀 Project Workflow

1. **Importing and Exploring Data**
   - Using `pandas` and `seaborn` for basic insights and visualizations
   - Understanding missing values and class distribution

2. **Data Cleaning/Preprocessing**
   - Null value treatment via mean replacement, flagging, or dropping
   - Data normalization if needed

3. **Model Building**
   - Supervised classification using algorithms like:
     - Logistic Regression
     - Decision Trees
     - Random Forest
     - Support Vector Machine (SVM)

4. **Model Evaluation**
   - Accuracy Score
   - Confusion Matrix
   - Classification Report (Precision, Recall, F1-Score)

5. **Comparative Results**
   - All three strategies are compared based on accuracy and performance

---

## 📊 Tools & Libraries Used

- **Python 3.x**
- **Pandas** for data manipulation
- **NumPy** for numeric processing
- **Seaborn** and **Matplotlib** for visualizations
- **Scikit-learn** for machine learning models and evaluation

---

## ▶️ How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/Ayush-k-Das/plant_disease_ML.git
   cd plant_disease_ML
