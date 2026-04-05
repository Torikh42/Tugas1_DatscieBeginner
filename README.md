# 🌸 Iris Flower Classification — Tugas 1
**Study Club Data Science Beginner**

Proyek ini bertujuan untuk mengklasifikasikan spesies bunga Iris (*Setosa, Versicolor, Virginica*) berdasarkan fitur pengukuran kelopak (*petal*) dan mahkota (*sepal*) bunga menggunakan algoritma Machine Learning.

---

### 📋 Informasi Proyek
- **Nama:** Torikh Abdullah Naser
- **Tugas:** Tugas 1 - Klasifikasi Dataset Publik
- **Dataset:** [Iris Flower Dataset](https://www.kaggle.com/datasets/uciml/iris) (Kaggle)

---

### 🛠️ Tech Stack & Library
Proyek ini dibangun menggunakan bahasa pemrograman **Python** dengan beberapa library utama:
- **Pandas**: Manipulasi dan analisis data tabular.
- **NumPy**: Komputasi numerik.
- **Matplotlib & Seaborn**: Visualisasi data dan hasil evaluasi.
- **Scikit-Learn**: Implementasi model Machine Learning (KNN & Random Forest), preprocessing, dan metrik evaluasi.

---

### ⚙️ Machine Learning Workflow
1. **Data Collecting**: Memuat dataset `Iris.csv`.
2. **Exploratory Data Analysis (EDA)**: Analisis statistik, korelasi antar fitur, dan visualisasi distribusi spesies.
3. **Data Preprocessing**: 
    - Label Encoding pada target (*Species*).
    - Train-Test Split (80% latih, 20% uji).
    - Feature Scaling menggunakan *StandardScaler*.
4. **Model Training**:
    - **K-Nearest Neighbors (KNN)**: Optimasi nilai K menggunakan Cross-Validation.
    - **Random Forest**: Implementasi Ensemble Learning dengan 100 decision trees.
5. **Model Evaluation**: Penilaian menggunakan Accuracy Score, Confusion Matrix, dan Classification Report.

---

### 📊 Hasil Akhir & Performa
Berdasarkan pengujian pada data uji (*test set*), berikut adalah performa model yang dihasilkan:

| Model | Test Accuracy | CV Mean Accuracy |
|---|---|---|
| **K-Nearest Neighbors (K=5)** | **93.33%** | **96.67%** |
| **Random Forest** | **90.00%** | **95.00%** |

#### **Insight Utama:**
- **Fitur Dominan**: `PetalLengthCm` dan `PetalWidthCm` merupakan fitur paling berpengaruh dalam klasifikasi.
- **Klasifikasi Spesies**: Spesies *Iris-setosa* berhasil diklasifikasikan dengan sempurna (100% precision & recall). Sedikit *overlap* terjadi pada *Versicolor* dan *Virginica*.
- **Model Terbaik**: KNN memberikan akurasi sedikit lebih tinggi pada dataset ini dibandingkan Random Forest.

---

### 📁 Struktur Folder
```text
Tugas1_TorikhAbdullahNaser/
├── Iris.csv                        # Dataset asli
├── Tugas1_DataScience_Iris.ipynb    # Notebook pengerjaan
└── README.md                       # Dokumentasi proyek
```

---

### 🚀 Cara Menjalankan
1. Pastikan Python terpasang di sistem Anda.
2. Instal library yang dibutuhkan:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```
3. Jalankan Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Buka file `Tugas1_DataScience_Iris.ipynb` dan jalankan semua cell.
