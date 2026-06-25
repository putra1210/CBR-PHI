# Case-Based Reasoning (CBR) untuk Putusan Perselisihan Hubungan Industrial (PHI)

## Deskripsi Proyek

Proyek ini merupakan implementasi **Case-Based Reasoning (CBR)** untuk menganalisis dan menemukan kemiripan pada putusan **Perselisihan Hubungan Industrial (PHI)** yang diperoleh dari **Direktori Putusan Mahkamah Agung Republik Indonesia**.

Metode yang digunakan pada proyek ini meliputi:

- Case Base Construction
- Case Representation
- Case Retrieval menggunakan **TF-IDF** dan **Cosine Similarity**
- Case Reuse menggunakan **Support Vector Machine (SVM)**
- Model Evaluation

---

# Struktur Repository

```text
CBR-PHI
│
├── data
│   ├── raw
│   ├── processed
│   ├── results
│   └── eval
│
├── notebooks
│   ├── 01_case_base.ipynb
│   ├── 02_case_representation.ipynb
│   ├── 03_case_retrieval.ipynb
│   ├── 04_case_solution_reuse.ipynb
│   └── 05_model_evaluation.ipynb
│
├── requirements.txt
└── README.md
```

---

# Dataset

Dataset yang digunakan berupa **30 Putusan Mahkamah Agung Republik Indonesia** kategori **Perselisihan Hubungan Industrial (PHI)** yang diperoleh dari **Direktori Putusan Mahkamah Agung Republik Indonesia**.

---

# Library yang Digunakan

Library yang digunakan dalam proyek ini meliputi:

- pandas
- numpy
- pdfplumber
- nltk
- Sastrawi
- scikit-learn
- matplotlib
- openpyxl

---

# Cara Instalasi

Clone repository:

```bash
git clone https://github.com/USERNAME/CBR-PHI.git
```

Masuk ke folder project:

```bash
cd CBR-PHI
```

Install seluruh dependency:

```bash
pip install -r requirements.txt
```

---

# Cara Menjalankan Program

Jalankan notebook secara berurutan:

### 1. 01_case_base.ipynb
- Mengekstrak file PDF menjadi dokumen teks.
- Melakukan pembersihan (cleaning) data.

### 2. 02_case_representation.ipynb
- Membentuk representasi kasus.
- Menghasilkan `cases.csv` dan `cases.json`.

### 3. 03_case_retrieval.ipynb
- Mengubah dokumen menjadi representasi TF-IDF.
- Menghitung tingkat kemiripan menggunakan Cosine Similarity.
- Menghasilkan `retrieval_results.csv`.

### 4. 04_case_solution_reuse.ipynb
- Mengimplementasikan tahap **Reuse** menggunakan **Support Vector Machine (SVM)**.
- Menghasilkan `prediction_results.csv`.

### 5. 05_model_evaluation.ipynb
- Menghitung Accuracy.
- Menghitung Precision.
- Menghitung Recall.
- Menghitung F1-Score.
- Menampilkan Confusion Matrix.
- Menghasilkan `evaluation.csv`.

---

# Metode yang Digunakan

- Case-Based Reasoning (CBR)
- TF-IDF (Term Frequency - Inverse Document Frequency)
- Cosine Similarity
- Support Vector Machine (SVM)

---

# Output Program

Output yang dihasilkan meliputi:

- `cases.csv`
- `cases.json`
- `retrieval_results.csv`
- `prediction_results.csv`
- `evaluation.csv`

---

# Anggota Kelompok

| No | Nama | NIM |
|----|-------------------------------|----------------|
| 1 | Putra Maulana Rahardiyanto | 202310370311249 |
| 2 | Fandy Rohman Sifa Aminulloh | 202310370311241 |

**Program Studi:** Informatika  
**Fakultas:** Fakultas Teknik  
**Universitas:** Universitas Muhammadiyah Malang

---

# Lisensi

Repository ini dibuat untuk memenuhi tugas mata kuliah **Penalaran Komputer** Program Studi Informatika Universitas Muhammadiyah Malang.
