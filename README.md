# Student Performance Prediction using Random Forest

[![Python](https://img.shields.io/badge/Python-3.13-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Latest-orange.svg)](https://scikit-learn.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📌 Deskripsi Proyek
Proyek ini bertujuan untuk memprediksi performa akademik siswa menggunakan algoritma **Random Forest**. Dengan menganalisis berbagai faktor seperti data demografis, kebiasaan belajar, dan latar belakang keluarga, model ini mampu mengklasifikasikan tingkat keberhasilan siswa dengan tingkat akurasi yang tinggi.

Pengerjaan dilakukan melalui pendekatan *end-to-end data science*, mulai dari eksplorasi data mentah hingga evaluasi model yang telah dioptimasi.

## 🚀 Alur Kerja (Methodology)
Proyek ini dibagi menjadi empat tahap utama yang didokumentasikan secara sistematis dalam direktori `notebooks/`:

1.  **Data Understanding**: Analisis awal dataset untuk memahami variabel, tipe data, dan distribusi awal.
2.  **Exploratory Data Analysis (EDA)**: Visualisasi mendalam untuk menemukan korelasi antar fitur dan mendeteksi pola yang memengaruhi performa siswa.
3.  **Data Preprocessing**: Pembersihan data, penanganan *outliers*, pengkodean variabel kategorikal, dan pembagian dataset (*train-test split*).
4.  **Modeling & Evaluation**: Implementasi model Random Forest dan evaluasi performa menggunakan metrik standar industri.

## 📊 Hasil & Evaluasi
Berdasarkan eksperimen terakhir, model Random Forest memberikan performa yang solid dalam memprediksi capaian akademik. Berikut adalah ringkasan metrik yang dicapai:

| Metric | Score |
| :--- | :--- |
| **Accuracy** | 0.91 |
| **Precision** | 0.89 |
| **Recall** | 0.90 |
| **F1-Score** | 0.89 |

*Detail lengkap performa model dapat dilihat pada file `outputs/model_metrics.json`.*

## 📈 Visualisasi Kunci
Analisis data menunjukkan beberapa poin penting:
* Korelasi kuat antara **Waktu Belajar (Study Time)** dan **Nilai Akhir**.
* Pengaruh signifikan tingkat pendidikan orang tua terhadap motivasi akademik siswa.
* Distribusi target menunjukkan klasifikasi yang seimbang untuk model prediksi.

---
