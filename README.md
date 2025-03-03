# Credit Risk Prediction

## Project Description
Proyek ini bertujuan untuk membangun model machine learning yang dapat memprediksi risiko kredit berdasarkan dataset pinjaman. Dengan model ini, perusahaan multifinance dapat meningkatkan keakuratan dalam menilai dan mengelola risiko kredit guna mengoptimalkan keputusan bisnis mereka.

## Latar Belakang
Dalam industri keuangan, menilai kelayakan kredit calon peminjam adalah tantangan besar. Dengan memanfaatkan data historis, machine learning dapat membantu dalam mengidentifikasi pola dan faktor risiko yang dapat meningkatkan efisiensi dalam proses pengambilan keputusan kredit.

## Dataset
Dataset yang digunakan berisi berbagai informasi pinjaman, termasuk:
- Jumlah pinjaman (loan_amnt)
- Tingkat suku bunga (int_rate)
- Status pekerjaan peminjam (emp_length)
- Pendapatan tahunan (annual_inc)
- Status pembayaran pinjaman sebelumnya (loan_status)

Dataset ini terdiri dari 75 kolom dengan total 39.834 entri.

## Problem Statement
Bagaimana cara membangun model machine learning yang dapat secara efektif memprediksi risiko kredit berdasarkan karakteristik peminjam?

## Data Understanding
Strategi eksplorasi data:
- Memahami struktur dataset dan distribusi data.
- Mengidentifikasi fitur yang paling relevan untuk prediksi risiko kredit.
- Melakukan visualisasi untuk mendapatkan wawasan awal.

### Contoh Eksplorasi Data
- **Korelasi antar variabel**: Menggunakan heatmap untuk melihat hubungan antar fitur.
- **Distribusi variabel numerik**: Menggunakan histogram dan boxplot untuk mendeteksi outlier.
- **Distribusi variabel kategorikal**: Menggunakan countplot untuk melihat distribusi kelas.

## Feature Engineering
Strategi yang digunakan:
- Mengonversi variabel kategorikal menjadi numerik menggunakan Label Encoding.
- Normalisasi fitur numerik menggunakan StandardScaler.
- Menangani nilai yang hilang dengan penghapusan atau imputasi.
- Menambahkan fitur baru seperti lama kredit berdasarkan issue_d dan earliest_cr_line.

### Seleksi Fitur
Fitur yang digunakan dalam model:
- `loan_amnt`, `funded_amnt`, `int_rate`, `installment`, `grade`, `sub_grade`
- `emp_length`, `home_ownership`, `annual_inc`, `verification_status`, `dti`
- `open_acc`, `revol_bal`, `revol_util`, `total_acc`, `loan_status`

## Exploratory Data Analysis (EDA)
- Korelasi antar variabel menggunakan heatmap.
- Histogram untuk melihat distribusi fitur numerik.
- Boxplot untuk mengidentifikasi outlier.
- Countplot untuk melihat distribusi grade pinjaman.

## Data Preparation
Langkah-langkah yang dilakukan:
- **Pembagian Data**: Dataset dibagi menjadi training dan testing set dengan rasio 80:20.
- **Scaling**: Menggunakan StandardScaler untuk memastikan model lebih stabil.
- **Penyesuaian Distribusi Kelas**: Jika terdapat ketidakseimbangan, dilakukan resampling.

## Model Training
Model yang digunakan:
- **Logistic Regression**
- **Random Forest**
- **Gradient Boosting**

Evaluasi model dilakukan menggunakan metrik:
- **Accuracy**
- **Precision & Recall**
- **F1-score**
- **ROC-AUC Curve**

## Kesimpulan
Dengan pendekatan ini, model dapat membantu perusahaan multifinance dalam menilai risiko kredit dengan akurasi 80%. Model yang dibangun dapat terus disempurnakan dengan data tambahan dan tuning parameter lebih lanjut.

## Dependencies
- Pandas
- Numpy
- Scikit-learn
- Seaborn
- Matplotlib

