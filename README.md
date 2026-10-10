# 📚 Scikit-Learn Cookbook

> Reproduksi kode dan pendalaman teori dari buku *scikit-learn Cookbook* (O'Reilly / Packt)

Kumpulan Jupyter Notebook yang mencakup alur machine learning dari preprocessing data sampai deployment model
menggunakan [scikit-learn](https://scikit-learn.org/). Repositori ini dibuat untuk *Tugas 2 – Enrichment for Machine Learning Classes*.
Setiap notebook berisi ringkasan bab, penjelasan teori (disusun dengan bantuan LLM), dan kode yang bisa langsung dijalankan
dengan dataset bawaan scikit-learn.

## 📖 Daftar Isi

| #  | Bab | Topik yang Dibahas | Status |
| --- | --- | --- | --- |
| 01 | [**API Elements of scikit-learn**](01.%20API%20Elements%20of%20scikit-learn/) | Estimator, transformer, pipeline, estimator kustom, pencarian hyperparameter, tag metadata | Selesai |
| 02 | [**Data Preprocessing**](02.%20Data%20Preprocessing/) | Imputasi, scaling, encoding kategori, ColumnTransformer, feature engineering | Selesai |
| 03 | [**Dimensionality Reduction**](03.%20Dimensionality%20Reduction/) | PCA, LDA, t-SNE, pengaruh terhadap performa model | Selesai |
| 04 | [**Models with Distance Metrics and Nearest Neighbors**](04.%20Models%20with%20Distance%20Metrics%20and%20Nearest%20Neighbors/) | Metrik jarak, KNN, penyetelan hyperparameter, evaluasi | Selesai |
| 05 | [**Linear Models and Regularization**](05.%20Linear%20Models%20and%20Regularization/) | Regresi linear, Ridge, Lasso, Elastic Net | Selesai |
| 06 | **Advanced Logistic Regression** | Klasifikasi biner & multikelas, regularisasi, evaluasi model | Tenggat 17 Okt 2026 |
| 07 | **Support Vector Machines and Kernel Methods** | SVM, fungsi kernel, penyetelan parameter | Tenggat 17 Okt 2026 |
| 08 | **Tree-Based Algorithms and Ensemble Methods** | Decision tree, Random Forest, Gradient Boosting | Tenggat 17 Okt 2026 |
| 09 | **Text Processing and Multiclass Classification** | Vektorisasi teks, ekstraksi fitur, klasifikasi teks | Menyusul |
| 10 | **Clustering Techniques** | K-Means, DBSCAN, hierarchical clustering | Menyusul |
| 11 | **Novelty and Outlier Detection** | Isolation Forest, One-Class SVM, LOF | Menyusul |
| 12 | **Cross-Validation and Model Evaluation** | K-Fold, seleksi model, generalisasi | Menyusul |
| 13 | **Deploying Models in Production** | Serialisasi model, pipeline untuk produksi, monitoring | Menyusul |

## 🔎 Gambaran Tiap Bab

**01. API Elements of scikit-learn.** Filosofi desain scikit-learn dan API intinya: estimator (`fit`), predictor (`predict`),
transformer (`transform`), estimator kustom, `Pipeline`, `GridSearchCV` / `RandomizedSearchCV`, atribut umum, tag estimator,
dan praktik terbaik penggunaan API.

**02. Data Preprocessing.** Dampak data mentah terhadap model dan cara memperbaikinya: mengenali masalah data, imputasi nilai hilang,
scaling (Standard, MinMax, Robust), encoding kategori (One-Hot, Ordinal), `ColumnTransformer`, feature engineering,
dan latihan preprocessing tanpa kebocoran data.

**03. Dimensionality Reduction.** Curse of dimensionality, **PCA** (memaksimalkan varians), **LDA** (memaksimalkan pemisahan kelas),
perbedaan keduanya, **t-SNE** untuk visualisasi, serta pengaruhnya terhadap akurasi dan waktu pelatihan.

**04. Models with Distance Metrics and Nearest Neighbors.** Metrik jarak (Euclidean, Manhattan, Minkowski, Chebyshev, cosine),
algoritma **KNN**, peran nilai *k* terhadap bias dan varians, pentingnya scaling, penyetelan hyperparameter, dan evaluasi
(confusion matrix, ROC-AUC, learning curve).

**05. Linear Models and Regularization.** OLS dan masalah overfitting, lalu **Ridge (L2)**, **Lasso (L1)**, dan **Elastic Net**:
coefficient path, memilih α dengan cross-validation, dan latihan klasifikasi Ridge serta Elastic Net.

**06–13.** Akan ditambahkan sesuai jadwal pengumpulan.

## 🚀 Memulai

### Prasyarat
- Python 3.8+
- Jupyter Notebook atau JupyterLab

### Instalasi
```bash
# Clone repositori
git clone https://github.com/<username>/scikit-learn-cookbook.git
cd scikit-learn-cookbook

# Install dependensi
pip install scikit-learn numpy pandas matplotlib scipy jupyter

# Jalankan Jupyter
jupyter notebook
```

### Dependensi Utama
| Package | Fungsi |
| --- | --- |
| `scikit-learn` | Algoritma machine learning dan utilitasnya |
| `numpy` | Komputasi numerik |
| `pandas` | Manipulasi dan analisis data |
| `matplotlib` | Visualisasi data |
| `scipy` | Distribusi statistik untuk pencarian hyperparameter |

## 🗂️ Struktur Repositori
```
scikit-learn-cookbook/
├── 01. API Elements of scikit-learn/
├── 02. Data Preprocessing/
├── 03. Dimensionality Reduction/
├── 04. Models with Distance Metrics and Nearest Neighbors/
├── 05. Linear Models and Regularization/
└── README.md
```
Setiap folder bab berisi notebook (`.ipynb`) dengan ringkasan, teori, kode, dan visualisasi.

## 🙏 Referensi
- [Dokumentasi scikit-learn](https://scikit-learn.org/stable/documentation.html)
- *scikit-learn Cookbook, Third Edition* – Packt Publishing / O'Reilly
