# 📊 Project ML Pemula: Klasifikasi Garis Kemiskinan

## 🧠 Deskripsi Proyek

Proyek ini merupakan bagian dari program Belajar Machine Learning Pemula (BMLP) yang diselenggarakan oleh Dicoding. Tujuan utama dari proyek ini adalah membangun model klasifikasi untuk mengelompokkan data garis kemiskinan berdasarkan jenis pengeluaran dan daerah. Proyek ini mencakup proses preprocessing data, pelatihan model dengan berbagai algoritma, evaluasi performa model, dan analisis hasil.

## 📁 Struktur Repositori

```
Project_ML_Pemula/
├── [Clustering]_Submission_Akhir_BMLP_Reza_Yasa_Putra.ipynb
├── [Klasifikasi]_Submission_Akhir_BMLP_Reza_Yasa_Putra.ipynb
├── garisKemiskinan.csv
├── garis_kemiskinan_clustering.csv
└── README.md
```

* `[Clustering]_Submission_Akhir_BMLP_Reza_Yasa_Putra.ipynb`: Notebook untuk proses clustering data.
* `[Klasifikasi]_Submission_Akhir_BMLP_Reza_Yasa_Putra.ipynb`: Notebook untuk proses klasifikasi data.
* `garisKemiskinan.csv`: Dataset awal yang digunakan.
* `garis_kemiskinan_clustering.csv`: Dataset hasil dari proses clustering yang digunakan untuk klasifikasi.

## Library yang dipakai

Proyek ini menggunakan bahasa pemrograman Python dengan bantuan beberapa library berikut:

* **Pandas**: Manipulasi dan analisis data.
* **NumPy**: Operasi numerik.
* **Matplotlib & Seaborn**: Visualisasi data.
* **Scikit-learn**: Algoritma machine learning dan evaluasi model.
* **Imbalanced-learn (SMOTE)**: Penanganan data yang tidak seimbang.

## 🧪 Proses dan Metodologi

1. **Import Library**: Mengimpor semua library yang diperlukan untuk analisis dan pemodelan.
2. **Memuat Dataset**: Membaca dataset hasil clustering ke dalam DataFrame.
3. **Preprocessing Data**:

  * Menghapus atau Menangani Data Kosong (Missing Values)
  * Menghapus Data Duplikat
  * Normalisasi atau Standarisasi Fitur
  * Deteksi dan Penanganan Outlier
  * Encoding Data Kategorikal
  * Binning (Pengelompokan Data)
4. **Splitting Data**: Membagi data menjadi data latih dan data uji dengan rasio 20:80.
5. **Handling Imbalanced Data**: Menggunakan SMOTE untuk menangani ketidakseimbangan kelas pada data latih.
6. **Modeling**: Melatih empat model klasifikasi:

   * K-Nearest Neighbors (KNN)
   * Decision Tree (DT)
   * Gaussian Naïve Bayes (NB)
   * Support Vector Machine (SVM)
7. **Evaluasi Model**:

   * Menghitung metrik evaluasi: Accuracy, Precision, Recall, dan F1-Score.
   * Menampilkan confusion matrix untuk masing-masing model.

## 📈 Hasil Evaluasi Model

| Model                        | Accuracy | Precision | Recall | F1-Score |
| ---------------------------- | -------- | --------- | ------ | -------- |
| K-Nearest Neighbors (KNN)    | 1.00     | 1.00      | 1.00   | 1.00     |
| Decision Tree (DT)           | 1.00     | 1.00      | 1.00   | 1.00     |
| Gaussian Naïve Bayes (NB)    | 1.00     | 1.00      | 1.00   | 1.00     |
| Support Vector Machine (SVM) | 1.00     | 1.00      | 1.00   | 1.00     |

> **Catatan**: Semua model menunjukkan performa sempurna pada data uji. Hal ini mungkin disebabkan oleh pola data yang sangat jelas atau fitur yang sangat informatif.

## 📊 Visualisasi Confusion Matrix

![Confusion Matrix](confusion_matrix.png)

> *Gambar di atas menunjukkan confusion matrix untuk masing-masing model, yang semuanya menunjukkan klasifikasi sempurna tanpa kesalahan.*

## 🧠 Analisis dan Insight

* **Overfitting**: Performa sempurna pada data uji dapat mengindikasikan overfitting. Diperlukan pengujian lebih lanjut dengan data baru untuk memastikan generalisasi model.
* **Kualitas Data**: Dataset yang digunakan memiliki pola yang sangat jelas, sehingga model dapat dengan mudah mempelajari dan mengklasifikasikan data.
* **Rekomendasi**:

  * Lakukan cross-validation untuk mengevaluasi konsistensi model.
  * Uji model dengan dataset lain untuk menguji generalisasi.
  * Pertimbangkan untuk menambahkan noise atau menggunakan dataset yang lebih kompleks.

## 🚀 Cara Menjalankan Proyek

1. **Clone Repository**:

   ```bash
   git clone https://github.com/Rezayasaputra29/Project_ML_Pemula.git
   cd Project_ML_Pemula
   ```

2. **Install Dependencies**:
   Pastikan Anda memiliki Python 3.x dan pip. Kemudian install dependencies dengan:

   ```bash
   pip install -r requirements.txt
   ```

   *Catatan: Jika file `requirements.txt` belum tersedia, Anda dapat menginstall library yang diperlukan secara manual.*

3. **Jalankan Notebook**:
   Buka notebook menggunakan Jupyter Notebook atau JupyterLab:

   ```bash
   jupyter notebook
   ```

   Kemudian buka file `[Klasifikasi]_Submission_Akhir_BMLP_Reza_Yasa_Putra.ipynb` untuk melihat proses klasifikasi.





