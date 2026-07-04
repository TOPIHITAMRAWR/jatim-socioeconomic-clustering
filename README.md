# 📍 Analisis Klasterisasi Kesejahteraan Kabupaten/Kota di Jawa Timur

Repositori ini berisi proyek riset analisis data untuk memetakan tingkat kesejahteraan antar kabupaten dan kota di Provinsi Jawa Timur. Proyek ini mengimplementasikan teknik *unsupervised machine learning* untuk mengelompokkan daerah-daerah berdasarkan berbagai indikator sosial dan ekonomi.

## 📊 Deskripsi Proyek
Ketimpangan kesejahteraan seringkali menjadi tantangan dalam pemerataan pembangunan. Analisis ini bertujuan untuk mengekstraksi wawasan dari data multi-dimensi indikator sosial-ekonomi Jawa Timur. Dengan menggunakan pendekatan berbasis *machine learning*, daerah dengan karakteristik serupa dikelompokkan ke dalam klaster tertentu, yang diharapkan dapat menjadi referensi objektif untuk pengambilan kebijakan atau analisis lanjutan.

## 🛠️ Metodologi yang Digunakan
1. **Exploratory Data Analysis (EDA):** Eksplorasi awal untuk memahami distribusi dan karakteristik data.
2. **Principal Component Analysis (PCA):** Teknik reduksi dimensi untuk menyederhanakan indikator sosial-ekonomi yang kompleks (multikolinearitas) menjadi beberapa komponen utama tanpa menghilangkan informasi krusial.
3. **K-Means Clustering:** Algoritma klasterisasi partisional untuk membagi daerah ke dalam kelompok kesejahteraan.
4. **Agglomerative (Hierarchical) Clustering:** Pendekatan klasterisasi hierarkis untuk memvalidasi dan membandingkan hasil struktur pengelompokan dari K-Means.

## 📁 Struktur File
*   `jatim_welfare_clustering.ipynb`: *Jupyter Notebook* utama yang berisi seluruh langkah analisis, mulai dari pra-pemrosesan data, pemodelan PCA, eksekusi algoritma K-Means & Agglomerative, hingga visualisasi hasil.
*   `Dataset Clustering.xlsx`: File *spreadsheet* mentah berisi metrik dan indikator sosial-ekonomi dari tiap kabupaten/kota di Jawa Timur yang digunakan dalam analisis.
*   `gadm41_IDN_2.zip`: Berkas *shapefile* (data spasial geospasial) batas wilayah administratif Indonesia. File ini digunakan di dalam *notebook* untuk memvisualisasikan hasil klasterisasi ke dalam bentuk peta (*choropleth map*) Jawa Timur.

## 🚀 Cara Menjalankan Proyek Lokal
Jika Anda ingin menjalankan *notebook* ini di komputer Anda sendiri:
1. Lakukan *clone repository* ini:
   ```bash
   git clone [https://github.com/TOPIHITAMRAWR/jatim-socioeconomic-clustering.git](https://github.com/TOPIHITAMRAWR/jatim-socioeconomic-clustering.git)


1. Pastikan Anda telah menginstal *library* Python berikut di lingkungan (*environment*) Anda:
   * `pandas` & `numpy` (Manipulasi data)
   * `scikit-learn` (Modeling PCA & Clustering)
   * `matplotlib` & `seaborn` (Visualisasi grafik)
   * `geopandas` (Untuk membaca file `.zip` spasial dan membuat peta)
2. Buka file `jatim_welfare_clustering.ipynb` menggunakan Jupyter Notebook atau VS Code.

---
**Pengembang**<br>
Ramadhan Adi Nugraha<br>
Mahasiswa Sains Data Terapan, Politeknik Elektronika Negeri Surabaya
