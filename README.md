# 🎓 Student Academic Performance Prediction

Sebuah **Micro Project Data Mining** yang memprediksi kategori nilai akademik siswa (`GradeClass`) berdasarkan fitur demografis, kebiasaan belajar, dan dukungan lingkungan. Proyek ini mengimplementasikan **Random Forest Classifier** untuk masalah klasifikasi multi-kelas, lengkap dengan pipeline EDA, preprocessing, evaluasi metrik, dan laporan akademik.

## 🔑 Fitur Utama
- 📊 **EDA Komprehensif**: Distribusi target, korelasi fitur, deteksi outlier
- 🧹 **Preprocessing**: Missing value check, stratified train-test split (80:20)
- 🌲 **Modeling**: Random Forest dengan feature importance analysis
- 📈 **Evaluasi**: Accuracy, Precision, Recall, F1-Score, Confusion Matrix
- 📄 **Dokumentasi**: Laporan lengkap (PDF/Word) + source code terstruktur

## 🛠️ Tech Stack
`Python 3.10` | `Pandas` | `NumPy` | `Scikit-learn` | `Matplotlib` | `Seaborn` | `Jupyter/VS Code`

## 📂 Struktur Project
📁 student-performance-prediction-rf/
├── 📄 README.md
├── 📄 environment.yml / requirements.txt
├── data/
│ ── 📄 raw/Student_performance_data.csv
├── notebooks/
│ ├── 01_Data_Understanding.ipynb
│ ├── 02_EDA_Visualization.ipynb
│ ├── 03_Data_Preprocessing.ipynb
│ └── 04_Modeling_Evaluation.ipynb
├── 📁 outputs/
│ ├── 📁 figures/
│ └── 📄 model_metrics.json
└── 📁 docs/
├── 📄 Laporan_Micro_Project.pdf
└── 📄 Slide_Presentasi.pdf

## 🚀 Quick Start
1. Clone repo: `git clone https://github.com/[username]/student-performance-prediction-rf.git`
2. Buat environment: `conda env create -f environment.yml`
3. Jalankan notebook secara berurutan dari `notebooks/`
