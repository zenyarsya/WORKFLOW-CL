# Repository Implementasi CI (Continuous Integration) - MLOps

Selamat datang di repository **WORKFLOW-CL**. Repository ini didedikasikan khusus untuk memenuhi kriteria implementasi **Continuous Integration (CI)** dalam siklus hidup MLOps.

## Deskripsi Proyek
Repository ini menyimpan konfigurasi otomatisasi menggunakan **GitHub Actions**. Tujuan utamanya adalah untuk memastikan bahwa setiap perubahan kode yang diunggah (push) ke repository utama akan melalui proses validasi otomatis untuk menjaga kualitas model dan integritas kode.

## Fitur Utama
* **Otomatisasi Validasi**: Menjalankan pengujian otomatis setiap kali ada perubahan pada script model.
* **Environment Setup**: Melakukan instalasi dependensi Python yang diperlukan seperti `pandas`, `scikit-learn`, dan `mlflow` secara otomatis.
* **Integrasi MLOps**: Dirancang untuk mendukung alur kerja eksperimen Machine Learning yang terhubung dengan MLflow dan DagsHub.

## Struktur Folder
* **`.github/workflows/`**: Berisi file konfigurasi YAML (misalnya `ci.yml`) yang menentukan instruksi kerja GitHub Actions.
* **`MLProject`**: File deskripsi lingkungan untuk standarisasi eksekusi model menggunakan MLflow.

## Cara Kerja
1. Pengembang melakukan *push* kode ke repository.
2. GitHub Actions secara otomatis memicu alur kerja yang didefinisikan dalam folder `.github/workflows/`.
3. Sistem akan menyiapkan lingkungan Python, menginstal dependensi, dan menjalankan pengujian script.
4. Status keberhasilan atau kegagalan akan ditampilkan pada tab **Actions**.
