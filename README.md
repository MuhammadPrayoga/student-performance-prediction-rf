# Student Performance Prediction 🎓📊

Proyek *Machine Learning* ini bertujuan untuk memprediksi performa atau klasifikasi nilai siswa (**Grade Class**) berdasarkan berbagai faktor pendukung seperti kebiasaan belajar, kehadiran, dan latar belakang sosial. 

Dengan model prediksi yang akurat, institusi pendidikan dapat melakukan identifikasi dini terhadap siswa yang berisiko mengalami penurunan nilai sehingga intervensi akademik dapat dilakukan lebih cepat dan tepat sasaran.

## 📌 Dataset Overview
Dataset yang dianalisis mencakup **2.392 data siswa** dengan **15 fitur** yang dikelompokkan menjadi:
- **Demografi & Latar Belakang:** `Age`, `Gender`, `Ethnicity`, `ParentalEducation`
- **Faktor Akademik:** `StudyTimeWeekly`, `Absences`, `Tutoring`, `GPA`
- **Faktor Non-Akademik:** `Extracurricular`, `Sports`, `Music`, `Volunteering`
- **Dukungan Sosial:** `ParentalSupport`
- **Target Variabel:** `GradeClass` (0: Nilai Tertinggi/A, hingga 4: Nilai Terendah/E)

## 🔍 Metodologi & Temuan (EDA)
Proses *Exploratory Data Analysis* (EDA) mengungkap beberapa karakteristik penting dari data siswa:
1. **Imbalanced Class:** Data sangat didominasi oleh siswa dengan nilai rendah (Grade 4.0 mencakup 50.6% populasi), sedangkan siswa unggulan (Grade 0.0) hanya 4.5%.
2. **Kualitas Data:** Tidak ditemukan anomali atau *outliers* (0.0%) pada fitur-fitur krusial seperti jam belajar mingguan, jumlah absensi, maupun GPA.
3. **Korelasi Target:** Waktu belajar (*StudyTimeWeekly*) dan GPA berkorelasi kuat dengan pencapaian Grade yang lebih baik, sedangkan jumlah ketidakhadiran (*Absences*) berkorelasi sangat kuat (0.72) dengan pemburukan nilai siswa.

## 🤖 Pemodelan (Random Forest)
Data dibagi menjadi 80% untuk *training* dan 20% untuk *testing*. Model yang digunakan adalah **Random Forest Classifier**.

**Hasil Evaluasi Model:**
- **Akurasi Keseluruhan:** **91.23%**
- **Performa Kelas:** Model sangat presisi dalam mengidentifikasi siswa di Grade 4.0 (*F1-Score: 0.96*), namun memiliki tantangan pada kelas minoritas seperti Grade 0.0 (*F1-Score: 0.44*) karena sifat data yang *imbalanced*.

**Top 3 Fitur Paling Berpengaruh (Feature Importance):**
1. `GPA` (Score: 0.503)
2. `Absences` (Score: 0.236)
3. `StudyTimeWeekly` (Score: 0.081)

## 💡 Kesimpulan & Rekomendasi
Dari analisis ini, terbukti bahwa performa siswa tidak terlalu bergantung pada faktor ekstrakurikuler atau demografi, melainkan sangat bergantung pada disiplin dan pondasi akademik dasar. 

**Rekomendasi:** Institusi pendidikan dan orang tua disarankan untuk lebih berfokus pada pemantauan tingkat kehadiran (mengurangi absen) serta mempertahankan nilai GPA dasar siswa untuk mencegah penurunan ke *Grade Class* yang lebih buruk.

---
