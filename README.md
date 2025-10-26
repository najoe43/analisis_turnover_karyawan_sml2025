# analisis_turnover_karyawan_sml2025
Proyek machine learning untuk memprediksi turnover karyawan berdasarkan dataset kompetisi Kaggle Tugas 1 SML A-2025
# Laporan Proyek Machine Learning  
## Prediksi Turnover Karyawan  
**Nama:** [Isi Nama Kamu]  
**NIM / ID:** [Isi NIM atau ID Kamu]  

---

## Daftar Isi  
- [Domain Proyek: Sumber Daya Manusia](#domain-proyek-sumber-daya-manusia)  
  - [Referensi](#referensi)  
- [Business Understanding](#business-understanding)  
  - [Problem Statements](#problem-statements)  
  - [Goals](#goals)  
- [Data Understanding](#data-understanding)  
- [Data Preparation](#data-preparation)  
- [Modeling](#modeling)  
- [Evaluation](#evaluation)  
- [Deployment / Kesimpulan](#deployment--kesimpulan)  

---

## Domain Proyek: Sumber Daya Manusia  
Proyek ini berfokus pada prediksi **turnover** atau perpindahan/keluar karyawan di sebuah organisasi menggunakan dataset kompetisi Kaggle “Tugas 1 SML A-2025”. Dataset ini mencakup profil karyawan, lingkungan kerja, dan status keluar atau tidak. :contentReference[oaicite:2]{index=2}  

### Referensi  
- Dataset: [Tugas 1 SML A-2025 – Kaggle](https://www.kaggle.com/competitions/tugas-1-sml-a-2025/data)  
- Dokumentasi/Instruksi kompetisi  
- Artikel/teori terkait turnover karyawan  

---

## Business Understanding  

### Problem Statements  
- Bagaimana memprediksi apakah seorang karyawan akan **keluar** dari organisasi (turnover) berdasarkan variabel yang tersedia?  
- Faktor‐faktor apa yang paling signifikan mempengaruhi keputusan karyawan untuk keluar?  

### Goals  
- Membangun model klasifikasi yang dapat memprediksi status keluar/karyawan bertahan dengan akurasi yang tinggi.  
- Mengidentifikasi fitur (variabel) utama yang menjadi indikator tinggi untuk turnover.  
- Menyajikan insight yang dapat digunakan oleh manajemen HR untuk mempertahankan karyawan.  

---

## Data Understanding  
Dataset terdiri dari [jumlah observasi jika diketahui] karyawan dengan sejumlah variabel demografis, jabatan, lingkungan kerja, dan status turnover. Contoh variabel:  
- `Age`  
- `JobRole`  
- `MonthlyIncome`  
- `YearsAtCompany`  
- `Attrition` (target: “Yes”/“No”)  

Pastikan kamu menyebutkan jumlah baris, jumlah variabel, missing values, dan sedikit gambaran distribusi.  

---

## Data Preparation  
Langkah‐langkah yang dilakukan:  
1. Menghapus atau mengisi missing values.  
2. Encoding variabel kategorik (misal JobRole, Gender, OverTime) ke numerik atau one‐hot.  
3. Normalisasi atau standardisasi fitur numerik (misal MonthlyIncome, YearsAtCompany).  
4. Menangani class imbalance jika target “Attrition: Yes” sangat sedikit (contoh: oversampling, undersampling).  
5. Split data ke train & test (misal 80% train, 20% test) atau menggunakan cross‐validation.  

---

## Modeling  
Model yang diuji:  
- Logistic Regression  
- Random Forest  
- XGBoost / LightGBM  
- (Opsional) Neural Network  

Model terbaik: **[Isi model terbaik]** dengan metrik akurasi / AUC / F1‐score terbaik.  
Contoh: “Random Forest mencapai akurasi 0.87 dan AUC 0.92”.

📌 Sertakan snippet kode atau diagram arsitektur (bila ada) untuk memperkuat dokumentasi.  

---

## Evaluation  
- Akurasi: [isi nilai]  
- Precision, Recall, F1 Score: [isi nilai masing‐masing]  
- ROC-AUC: [isi nilai]  
- Confusion Matrix:  
  ```markdown
  ![Confusion Matrix](img/confusion_matrix.png)
