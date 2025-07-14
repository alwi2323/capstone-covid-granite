# 🧠 Capstone Project: COVID-19 Data Classification and Summarization using IBM Granite

Proyek ini bertujuan untuk melakukan klasifikasi dan ringkasan data COVID-19 di Indonesia menggunakan metode analisis manual serta dukungan AI generatif dari model Granite IBM WatsonX.

---

## 🗂️ Dataset

**Nama:** COVID-19 Indonesia Time Series All  
**Sumber:** [Kaggle / Open Data](https://www.kaggle.com/datasets)  
**Link Dataset Lokal:** `data/covid_19_indonesia_time_series_all.csv`  
**Format:** CSV  
**Isi:** Data harian COVID-19 per provinsi di Indonesia, termasuk jumlah kasus baru, kematian, dan kesembuhan.

---

## 🧪 Analisis & Metodologi

Analisis dilakukan melalui beberapa tahap, antara lain:

- **Preprocessing & Cleaning:** Pembersihan data untuk kolom yang relevan seperti tanggal, provinsi, kasus, kematian, dan sembuh.
- **Perhitungan Tambahan:**  
  - Fatality rate (tingkat kematian)  
  - Recovery rate (tingkat kesembuhan)  
- **Klasifikasi Risiko:**  
  Provinsi diklasifikasikan ke dalam *Low*, *Medium*, atau *High Risk* berdasarkan jumlah kasus harian dan fatality rate.
- **Visualisasi:**  
  Menggunakan *seaborn* untuk melihat distribusi provinsi berdasarkan level risiko.
- **Summarization AI:**  
  Menggunakan model `granite-3-3-8b-instruct` dari IBM WatsonX Prompt Lab untuk menghasilkan ringkasan naratif dari data provinsi terpilih.

---

## 📊 Insight & Findings

Berikut adalah insight yang diperoleh dari hasil klasifikasi manual dan bantuan AI Granite dari IBM WatsonX:

### 🔹 Ringkasan Granite untuk DKI Jakarta – Juli 2021

> Dalam bulan Juli 2021, Provinsi DKI Jakarta mencatat perkembangan COVID-19 yang bervariasi.  
> Selama masa tersebut, terdapat 15.480 kasus baru, dengan 540 kematian baru, menunjukkan tingginya jumlah kematian bulanan.  
> Namun, jumlah pasien sembuh baru mencapai 13.920, menunjukkan tingkat kesembuhan yang tinggi sebesar 89.9%.  
> Rata-rata kasus harian di Jakarta tersebut mencapai 499, dan tingkat fatalitas terhadap kasus baru mencapai 3.49%.  
> Perkembangan ini menunjukkan situasi yang kritis, namun juga menandai potensi peningkatan sembuh di provinsi tersebut.

📌 *Model digunakan: `granite-3-3-8b-instruct`, IBM WatsonX Prompt Lab*

---

## 📂 Struktur Repository

