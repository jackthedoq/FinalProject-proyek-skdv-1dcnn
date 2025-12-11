# 🧠 SKDV Classification with 1D-CNN

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0%2B-orange?style=for-the-badge&logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-Red?style=for-the-badge&logo=keras)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

> **Final Project - Jaringan Syaraf Tiruan (JST)**
> Implementasi Deep Learning menggunakan arsitektur *One-Dimensional Convolutional Neural Network* (1D-CNN) untuk analisis data SKDV.

---

## 📝 Deskripsi & Kesimpulan Proyek

Secara keseluruhan, pengembangan sistem deteksi pada proyek SKDV ini mengimplementasikan arsitektur *Deep Learning* berbasis **1D-CNN (One-Dimensional Convolutional Neural Network)** yang dirancang khusus untuk menangani data sekuensial. 

Proses dimulai dari tahapan *preprocessing* data yang meliputi normalisasi dan *reshaping* dimensi input, dilanjutkan dengan pembangunan model yang memanfaatkan lapisan konvolusi 1D untuk mengekstraksi fitur pola lokal secara otomatis dari sinyal data. Kompleksitas fitur kemudian direduksi melalui lapisan *pooling* sebelum diproses oleh lapisan *fully-connected* untuk penentuan klasifikasi akhir. 

Berdasarkan hasil pelatihan dan evaluasi, model 1D-CNN ini terbukti mampu mempelajari karakteristik data SKDV dengan efektif, yang ditunjukkan oleh konvergensi nilai *loss* pelatihan yang stabil serta pencapaian metrik akurasi yang optimal pada data pengujian.

---

## 🛠️ Detail Arsitektur Model

Model dibangun menggunakan `TensorFlow/Keras` dengan alur sebagai berikut:

1.  **Input Layer**: Menerima data sekuensial (dimensi *Time Steps* x *Features*).
2.  **Conv1D Layers**: Melakukan ekstraksi fitur spasial/temporal menggunakan filter konvolusi yang bergerak satu arah.
3.  **MaxPooling1D**: Merupakan tahap *downsampling* untuk mereduksi dimensi fitur, mengurangi beban komputasi, dan mencegah *overfitting*.
4.  **Flatten**: Mengubah matriks fitur hasil *pooling* menjadi vektor satu dimensi.
5.  **Dense Layers**: Lapisan *Fully Connected* untuk klasifikasi akhir menggunakan fungsi aktivasi (misal: Softmax/Sigmoid).

---

## 🚀 Cara Menjalankan (Getting Started)

Ikuti langkah-langkah ini untuk menjalankan proyek di komputer lokal Anda:

### 1. Clone Repository
```bash
git clone [https://github.com/jackthedoq/FinalProject-proyek-skdv-1dcnn.git](https://github.com/jackthedoq/FinalProject-proyek-skdv-1dcnn.git)
cd FinalProject-proyek-skdv-1dcnn
