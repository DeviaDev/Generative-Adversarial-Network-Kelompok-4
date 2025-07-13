# 🧠 Generative Adversarial Network (GAN) – Kelompok 4

Proyek ini merupakan implementasi sederhana dari Generative Adversarial Network (GAN) menggunakan PyTorch, sebagai bagian dari tugas kelompok pada mata kuliah *Deep Learning*.

## 📌 Tujuan Proyek

- Memahami konsep dasar GAN
- Membangun arsitektur sederhana Generator dan Discriminator
- Melatih GAN pada dataset MNIST
- Menghasilkan gambar baru menyerupai angka tulisan tangan

## 👥 Anggota Kelompok

1. Devianest Narendra – 442023618087
2. Zainab Ahmad – 442023618107
3. Naila Fatikhah – 442023618086
4. Adya Rusmalillah – 442023618093

> Semua anggota berkontribusi aktif dalam pengembangan kode, dokumentasi, dan laporan. Riwayat commit di GitHub mencerminkan pembagian kerja yang adil.


## 🧬 Dataset

Kami menggunakan dataset **MNIST** (angka tulisan tangan) dari `torchvision.datasets`.

- Ukuran gambar: 28x28 piksel, grayscale
- Gambar dinormalisasi ke [-1, 1] untuk digunakan dengan aktivasi `Tanh`

## ⚙️ Arsitektur GAN

### Generator
- Input: noise vektor (100 dimensi)
- Output: gambar 28x28
- Aktivasi akhir: `Tanh`

### Discriminator
- Input: gambar 28x28
- Output: nilai probabilitas real/fake
- Aktivasi akhir: `Sigmoid`

## 📈 Hasil

- Visualisasi loss dari Generator dan Discriminator ditampilkan dalam notebook
- Gambar hasil disimpan dalam folder `generated_images/`
- Generator menunjukkan peningkatan hasil dari epoch ke epoch
- Model disimpan di folder `models/`

## 🚀 Cara Menjalankan

1. Pastikan Anda memiliki Python 3.8+ dan library: `torch`, `torchvision`, `matplotlib`
2. Jalankan file `implementasi-generative-adversarial-network-gan.ipynb` secara berurutan
3. Hasil gambar akan tersimpan otomatis ke folder `generated_images/`

### 📦 Requirements (jika dibutuhkan)

```bash
pip install torch torchvision matplotlib


