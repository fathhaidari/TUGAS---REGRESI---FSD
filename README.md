# Tugas Praktikum: Linear Regression dan Logistic Regression

---

## Identitas Mahasiswa
- **Nama**: Muhammad Fath Haidari
- **NIM**: 25523167
- **Kelas**: A

---

## Sumber Dataset

1. **Bagian A (Linear Regression)**
   - **Dataset**: California Housing Dataset (`sklearn.datasets.fetch_california_housing`)
   - **Tautan Sumber**: [Scikit-Learn California Housing Documentation](https://scikit-learn.org/stable/datasets/real_world.html#california-housing-dataset)
   - **Deskripsi**: Dataset berisi data sensus California tahun 1990 untuk memprediksi harga median rumah (`MedHouseVal`) berdasarkan 8 fitur prediktor seperti median pendapatan, umur rumah, dan lokasi geospasial[cite: 1].

2. **Bagian B (Logistic Regression)**
   - **Dataset**: Breast Cancer Wisconsin Dataset (`sklearn.datasets.load_breast_cancer`)
   - **Tautan Sumber**: [Scikit-Learn Breast Cancer Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html)
   - **Deskripsi**: Dataset diagnostik medis berisi 30 fitur pengukuran fisik sel untuk mengklasifikasikan kategori tumor menjadi **Ganas (Malignant / 0)** atau **Jinak (Benign / 1)**[cite: 1].

---

## Ringkasan Hasil Pemodelan

### 1. Bagian A: Linear Regression (Prediksi Harga Rumah)
- **Target**: `MedHouseVal` (Kontinu)
- **Evaluasi Data Uji**:
  - **MAE (Mean Absolute Error)**: ~0.36
  - **RMSE (Root Mean Squared Error)**: ~0.52
  - **R-squared (R²)**: ~0.58 (Model menjelaskan 58% variansi harga rumah)
- **Temuan Utama**: Fitur `MedInc` (median pendapatan) memiliki pengaruh paling dominan terhadap peningkatan harga rumah.

### 2. Bagian B: Logistic Regression (Klasifikasi Kanker Payudara)
- **Target**: `target` (Biner: 0 = Malignant, 1 = Benign)
- **Evaluasi Data Uji**:
  - **Accuracy**: 96.49%
  - **Precision**: 95.89%
  - **Recall**: 98.59%
  - **F1-Score**: 97.22%
  - **ROC-AUC**: 0.9912
- **Temuan Utama**: Nilai Recall yang sangat tinggi (~98.6%) menunjukkan model sangat handal dalam meminimalisir kesalahan diagnosa False Negative pada pasien medis.

---

## Rincian Kontribusi
Dikarenakan pengerjaan tugas dilakukan secara mandiri, seluruh tahapan proyek dikerjakan secara utuh oleh **Muhammad Fath Haidari**:
1. Penyiapan dataset, eksplorasi data (EDA), preprocessing, pemodelan, dan evaluasi pada notebook Bagian A (`A_linear_regression.ipynb`)[cite: 1].
2. Penyiapan dataset, eksperimen klasifikasi, analisis *Confusion Matrix*, dan kurva ROC pada notebook Bagian B (`B_logistic_regression.ipynb`)[cite: 1].
3. Penyusunan repositori GitHub, pengelolaan berkas notebook, dan dokumentasi proyek pada `README.md`[cite: 1].
