# 🍊 Citrus Fruit Classification: Orange vs. Grapefruit

![Python](https://img.shields.io/badge/Python-3.11-blue.svg?style=flat-square&logo=python)
![Jupyter Notebook](https://img.shields.io/badge/Tools-Jupyter_Notebook-orange.svg?style=flat-square&logo=jupyter)
![scikit-learn](https://img.shields.io/badge/Library-Scikit_Learn-yellow.svg?style=flat-square&logo=scikitlearn)
![Status](https://img.shields.io/badge/Status-Completed-success.svg?style=flat-square)

---

## 📌 Deskripsi Proyek

Proyek ini merupakan implementasi model *Machine Learning* untuk mengklasifikasikan jenis buah sitrus antara **Jeruk (Orange)** dan **Grapefruit** berdasarkan fitur fisik dan komposisi warna RGB.

Pengembangan ini dilakukan untuk memenuhi tugas **Ujian Tengah Semester (UTS)** dengan menerapkan metodologi standar industri **CRISP-DM** (*Cross-Industry Standard Process for Data Mining*).

---

## 📂 Struktur Proyek

```text
📦 UTS_AI_Klasifikasi
 ┣ 📜 klasifikasi.ipynb   # Notebook utama (Eksplorasi, Preprocessing & Modeling)
 ┣ 📜 citrus.csv          # Dataset Oranges vs Grapefruit
 ┗ 📜 README.md           # Dokumentasi proyek
```

---

## 📊 Dataset

Dataset diperoleh dari Kaggle: [Oranges vs Grapefruit](https://www.kaggle.com/datasets/joshmcadams/oranges-vs-grapefruit)

| Atribut | Detail |
| :--- | :--- |
| **Total Sampel** | 10.000 data (5.000 Orange, 5.000 Grapefruit) |
| **Distribusi Kelas** | Seimbang (50:50) |
| **Missing Values** | Tidak ada |

### Fitur Prediktor

| Fitur | Deskripsi |
| :--- | :--- |
| `diameter` | Diameter buah (cm) |
| `weight` | Berat buah (gram) |
| `red` | Komposisi warna merah (RGB) |
| `green` | Komposisi warna hijau (RGB) |
| `blue` | Komposisi warna biru (RGB) |

---

## ⚙️ Metodologi (CRISP-DM)

### 1. 🔍 Data Understanding
Identifikasi tipe data dan pengecekan statistik deskriptif untuk memastikan kualitas data awal.

### 2. 🛠️ Data Preparation
- **Label Encoding** — Transformasi kolom target (`Orange: 0`, `Grapefruit: 1`)
- **Data Splitting** — Pembagian dataset: **80% Training** | **20% Testing**
- **Feature Scaling** — Standardisasi menggunakan `StandardScaler` untuk mengoptimalkan kinerja algoritma berbasis jarak dan gradien

### 3. 🤖 Modeling
Tiga algoritma dilatih dan dibandingkan performanya:

| # | Algoritma |
| :---: | :--- |
| 1 | Decision Tree Classifier |
| 2 | Gaussian Naive Bayes |
| 3 | Support Vector Machine (SVM) |

### 4. 📈 Evaluation
Pengujian model menggunakan *Testing Set* dengan metrik: **Akurasi**, **Precision**, **Recall**, dan **F1-Score**.

---

## 🏆 Hasil Evaluasi Model

| Algoritma | Akurasi | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **Decision Tree** ⭐ | **94.40%** | **0.94** | **0.94** | **0.94** |
| Support Vector Machine (SVM) | 93.70% | 0.94 | 0.94 | 0.94 |
| Naive Bayes | 92.00% | 0.92 | 0.92 | 0.92 |

> **✅ Kesimpulan:** Model **Decision Tree** memberikan performa terbaik dengan akurasi **94.40%**. Model ini efektif dalam menangkap pola non-linear pada fitur diameter dan berat buah.

---

## 🚀 Panduan Instalasi & Penggunaan

### Prasyarat
- Python **3.8+**
- Visual Studio Code + ekstensi Jupyter

### Langkah Eksekusi

**1. Clone repositori**
```bash
git clone https://github.com/rhannalfa/UTS-ML.git
cd UTS-ML
```

**2. Instalasi dependensi**
```bash
pip install pandas scikit-learn ipykernel
```

**3. Jalankan notebook**

Buka `klasifikasi.ipynb` di VS Code, pilih kernel `.venv` atau Python global, lalu klik **Run All**.

---

## 👤 Informasi Pengembang

| | |
| :--- | :--- |
| **Nama** | Raihan Alfarizi |
| **Tugas** | Ujian Tengah Semester — Kecerdasan Buatan |
| **Tanggal** | April 2026 |
| **GitHub** | [@rhannalfa](https://github.com/rhannalfa) |
