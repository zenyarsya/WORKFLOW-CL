# Proyek MLOps: Segmentasi Pelanggan Retail (Customer Segmentation)

Proyek ini merupakan implementasi siklus hidup Machine Learning (MLOps) yang mencakup manajemen eksperimen, pelacakan model, hingga otomatisasi pengujian kode menggunakan standar industri.

## 📂 Struktur Repository Utama
- **`membangun_model/`**: Berisi seluruh aset pengembangan model, termasuk script pelatihan (`modelling.py`), file dependensi (`requirements.txt`), serta artefak dan metadata dari MLflow.
- **`Monitoring_dan_Logging/`**: Berisi script untuk menjalankan prediksi (inference) serta bukti visual bahwa model berhasil melayani permintaan data (serving) dan dipantau secara berkala.

## 🚀 Komponen Terintegrasi (Kriteria Submission)
Untuk memenuhi persyaratan submission Dicoding, proyek ini terhubung dengan repository pendukung berikut:

1. **Kriteria 1 (Eksperimen ML)**:
   Seluruh riwayat eksperimen dan preprocessing data dapat diakses pada repository khusus eksperimen:
   👉 [Repository Eksperimen SML](https://github.com/zenyarsya/Eksperimen_SML_Zeny-Arsya-Fortilla)

2. **Kriteria 3 (Implementasi CI/CD)**:
   Otomatisasi pengujian (Continuous Integration) dibangun secara mandiri menggunakan GitHub Actions dan MLflow Project untuk memastikan standarisasi lingkungan eksekusi:
   👉 [Repository Workflow CI (WORKFLOW-CL)](https://github.com/zenyarsya/WORKFLOW-CL)

## 🛠️ Teknologi yang Digunakan
- **Python & Scikit-Learn**: Digunakan untuk pemrosesan data dan pemodelan Clustering.
- **MLflow**: Digunakan untuk tracking eksperimen, pencatatan parameter, dan registrasi model.
- **DagsHub**: Sebagai remote storage untuk artefak model dan server pelacakan eksperimen.
- **GitHub Actions**: Menjalankan validasi kode secara otomatis melalui file `.github/workflows/ci.yml`.
