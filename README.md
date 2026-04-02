# Hyperparameter Tuning Project

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

Proyek ini merupakan praktikum Machine Learning yang berfokus pada optimasi model menggunakan teknik hyperparameter tuning pada dua jenis permasalahan:
- Regresi (Fuel Consumption Dataset)
- Klasifikasi (Hepatitis Dataset)

---

## Project Highlights

- Implementasi lengkap pipeline Machine Learning (EDA → preprocessing → modeling → tuning → evaluation)
- Perbandingan 4 metode hyperparameter tuning:
  - Grid Search
  - Random Search
  - Bayesian Optimization
  - Optuna
- Penanganan data imbalance menggunakan SMOTE
- Evaluasi model menggunakan metrik yang sesuai untuk masing-masing kasus
- Analisis learning curve untuk melihat generalisasi model

---

## Tujuan

Tujuan dari proyek ini adalah:
- Membangun model baseline
- Melakukan preprocessing data
- Menangani missing value, outlier, dan imbalance
- Mengoptimalkan performa model melalui hyperparameter tuning

---

## Dataset

### Fuel Consumption (Regresi)
- Jumlah data: 955
- Jumlah fitur: 14
- Target: CO2 Emissions
- Tidak terdapat missing value

### Hepatitis (Klasifikasi)
- Jumlah data: 154
- Jumlah fitur: 20
- Target: Class (0/1)
- Terdapat missing value dan ketidakseimbangan kelas

---

## Data Preprocessing

### Regresi
- StandardScaler (numerik)
- OneHotEncoder (kategorikal)

### Klasifikasi
- Missing value:
  - Numerik → Median
  - Kategorikal → Modus
- Outlier:
  - Capping (IQR)
- Imbalance:
  - SMOTE

---

## Model

### Regresi
- Linear Regression
- Ridge Regression
- Lasso Regression

### Klasifikasi
- Logistic Regression
- KNN
- SVM

---

## Evaluasi

### Regresi
- RMSE
- R² Score

### Klasifikasi
- Accuracy
- Precision
- Recall
- F1-Score

---

## Hyperparameter Tuning

Metode yang digunakan:
- Grid Search
- Random Search
- Bayesian Optimization
- Optuna

---

## Hasil

### Regresi
Ridge Regression memberikan performa terbaik dengan R² ≈ 0.997 setelah tuning.

### Klasifikasi
SVM menjadi model terbaik dengan F1-score ≈ 0.957 (Random Search) setelah penanganan imbalance.

---

## Insight

- Hyperparameter tuning meningkatkan performa model secara signifikan
- Model default belum tentu optimal
- Random Search dan Bayesian Optimization lebih efisien dibanding Grid Search
- Penanganan imbalance penting untuk klasifikasi

---

## Kesimpulan

Pada regresi, model Ridge memberikan performa terbaik dengan hasil yang stabil setelah tuning.  
Pada klasifikasi, kombinasi SVM, SMOTE, dan tuning menghasilkan model yang paling optimal dalam menangani data tidak seimbang.

---

## Tools

- Python
- Scikit-learn
- Imbalanced-learn
- Optuna
- Scikit-optimize
- Pandas, NumPy
- Matplotlib, Seaborn

---

## Author

Randi  
https://github.com/RandiBro234
