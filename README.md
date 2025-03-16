# 💡 **Analisis Umpan Balik Pelanggan dan Efisiensi Produksi pada DataCo Smart Supply Chain**

### **Dibuat oleh:**
- Winston Narada Kusumahadi
- Bryant Gabriel Effendi
- Farrany Sucitra Kusumahadi

## 📑 **Deskripsi Proyek**
Proyek ini bertujuan untuk menganalisis umpan balik pelanggan dan efisiensi produksi pada **DataCo Smart Supply Chain**. Dengan menggunakan data yang tersedia, proyek ini mengevaluasi kualitas layanan pengiriman dan memodelkan klasterisasi pelanggan serta efisiensi produksi. 

### 🎯 **Tujuan Utama:**
1. Mengelompokkan pelanggan berdasarkan karakteristik dan umpan balik mereka.
2. Mengukur efisiensi pengiriman dengan menghitung *Mean Absolute Percentage Error* (MAPE).
3. Menghitung risiko keterlambatan pengiriman dengan *Log Loss*.
4. Mengidentifikasi hubungan antar variabel melalui eksplorasi data.

---------------------------------------------------------

## ⚙️ **Teknik dan Model yang Digunakan**

### 🔍 **1. Exploratory Data Analysis (EDA)**
- Melakukan analisis statistik deskriptif untuk memahami distribusi data.
- Mengidentifikasi data yang hilang (*missing values*) dan outlier.
- Visualisasi data dengan *heatmap* dan *histogram* untuk memetakan korelasi antar fitur.

### 🧠 **2. Clustering dengan K-Means**
- Menggunakan metode *K-Means Clustering* untuk mengelompokkan data berdasarkan kesamaan fitur.
- Evaluasi hasil clustering dengan metrik berikut:
  - **Davies-Bouldin Index:** Mengukur seberapa baik kluster terbentuk.
  - **Calinski-Harabasz Index:** Mengukur kepadatan dan pemisahan kluster.

### 📈 **3. Evaluasi Model**
- Menghitung **MAPE (Mean Absolute Percentage Error)** untuk memprediksi efisiensi pengiriman.
- Menghitung **Log Loss** untuk memperkirakan risiko keterlambatan pengiriman.

### 🗃️ **4. Dimensionality Reduction dengan PCA**
- Menggunakan *Principal Component Analysis (PCA)* untuk mereduksi dimensi data sehingga dapat divisualisasikan dalam 2D.

---------------------------------------------------------

## 📝 **Struktur Proyek**
```bash
├── data.ipynb 
├── data/ # Folder dataset
    ├── Dataset_Pertama.csv
    └── Dataset_Kedua.csv 
├── models/ # Folder untuk menyimpan model yang sudah dilatih
    ├── kmeans_model.pkl
    └── scaler.pkl
├── results/ # Folder untuk hasil clustering dan analisis
    └── hasil_clustering.csv
├── README.md # Dokumentasi proyek
```

---------------------------------------------------------

## 🚀 **Cara Menjalankan Proyek**

### ✅ **Persyaratan:**
Pastikan Anda memiliki Python versi 3.8 atau lebih baru. 

### 🔧 **1. Mengkloning Repositori:**
```bash
git clone https://github.com/username/DataCo-SupplyChain-Analysis.git
cd DataCo-SupplyChain-Analysis
```

### 📦 **2. Menginstal Pustaka:**
```bash
pip install pandas
pip install numpy
pip install seaborn
pip install matplotlib
pip install scikit-learn
pip install joblib
```

### ▶️ **3. Menjalankan Analisis:**
Data dijalankan dalam data.ipynb

## 📂 **4. Output**
Setelah menjalankan kode, Anda akan mendapatkan beberapa file output, antara lain:

- **hasil_clustering.csv:** Hasil clustering dengan label kluster.
- **kmeans_model.pkl:** Model *K-Means* yang telah dilatih.
- **scaler.pkl:** Model *Standard Scaler* yang digunakan.
- **Visualisasi Grafis:** Grafik clustering dan korelasi disimpan sebagai gambar.

## 📊 **5. Hasil Evaluasi**
Berikut adalah hasil evaluasi model clustering dan prediksi:

- **Davies-Bouldin Index:** Mengukur validitas kluster (Semakin rendah semakin baik).
- **Calinski-Harabasz Index:** Mengukur pemisahan kluster (Semakin tinggi semakin baik).
- **MAPE (Mean Absolute Percentage Error):** Mengukur akurasi prediksi waktu pengiriman.
- **Log Loss:** Mengukur risiko keterlambatan pengiriman.

---

## 📚 **Referensi**
Dokumentasi pustaka yang digunakan dalam proyek ini:
- [Scikit-learn Documentation](https://scikit-learn.org/)
- [Pandas Documentation](https://pandas.pydata.org/)
- [Seaborn Documentation](https://seaborn.pydata.org/)
- [Joblib Documentation](https://joblib.readthedocs.io/)




