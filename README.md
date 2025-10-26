# analisis_attrition_karyawan_sml2025
Proyek machine learning untuk memprediksi turnover karyawan berdasarkan dataset kompetisi Kaggle Tugas 1 SML A-2025
# Laporan Proyek Machine Learning 

## Prediksi Turnover Karyawan  
**Nama:**
1. Najwa Allena Eka P.S (5003231025)
2. Najwa Putri Lathifah (5003231026)
3. Raisa Dinar Izzati (5003231028)
   
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
Proyek ini berfokus pada prediksi **turnover** atau perpindahan/keluar karyawan di sebuah perusahaan menggunakan dataset kompetisi Kaggle “Tugas 1 SML A-2025”. Dataset ini mencakup profil karyawan, lingkungan kerja, dan status keluar atau tidak. :contentReference[oaicite:2]{index=2}  

### Referensi  
- Dataset: [Tugas 1 SML A-2025 – Kaggle](https://www.kaggle.com/competitions/tugas-1-sml-a-2025/data)  

---

## Business Understanding  

### Problem Statements  
Tingkat keluar-masuk karyawan (attrition) merupakan salah satu permasalahan penting bagi perusahaan karena dapat menimbulkan kerugian, baik dari segi biaya rekrutmen, pelatihan, maupun penurunan produktivitas kerja. Ketika banyak karyawan yang keluar, proses adaptasi dan efisiensi tim jadi terganggu. Oleh karena itu, perusahaan perlu memahami faktor-faktor yang memengaruhi keputusan karyawan untuk keluar dan memprediksi kemungkinan tersebut sedini mungkin agar dapat dicegah sedini mungkin.

### Goals   
- Membuat model untuk memprediksi apakah seorang karyawan akan keluar dari perusahaan atau tidak.
- Mengetahui faktor-faktor apa saja yang paling berpengaruh terhadap keputusan karyawan keluar.
- Menghasilkan model dengan performa optimal menggunakan pendekatan hyperparameter tuning (GridSearchCV) dan evaluasi berbasis metrik AUC, akurasi, presisi, recall, serta F1-score.
- Memberikan saran yang dapat membantu HR dalam menjaga karyawan tetap bertahan di perusahaan.

---

## Data Understanding  
Dataset yang digunakan pada proyek ini diperoleh dari situs [Tugas 1 SML A-2025 – Kaggle](https://www.kaggle.com/competitions/tugas-1-sml-a-2025/data). 
Dataset ini terdiri dari 1170 data karyawan yang berisi 31 variabel seperti
- `Age`  
- `JobRole`  
- `MonthlyIncome`  
- `YearsAtCompany`  
- `Attrition` (target: “Yes”/“No”)
- dan variabel yang lainnya

---

## Data Preparation  
Langkah‐langkah yang dilakukan:  
1. Menghapus atau mengisi missing values.  
2. Encoding variabel kategorik (misal JobRole, Gender, OverTime) ke numerik atau one‐hot.  
3. Normalisasi atau standardisasi fitur numerik (misal MonthlyIncome, YearsAtCompany).  
4. Menangani class imbalance jika target “Attrition: Yes” sangat sedikit (contoh: oversampling, undersampling).  
5. Split data ke train & test (misal 80% train, 20% test) atau menggunakan cross‐validation.  

### Histogram Semua Variabel Numerik
![Histogram Semua Variabel Numerik](C:\Users\NAJWA\Pictures\Screenshots\Screenshot 2025-10-26 191202.png)
---

## Modelling  
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
