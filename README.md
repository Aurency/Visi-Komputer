# Deteksi Stomata pada Citra Mikroskopis Daun Menggunakan Segmentasi Thresholding dan Morfologi

Proyek ini merupakan bagian dari tugas akhir mata kuliah Visi Komputer Semester Genap Tahun Akademik 2024/2025. Tujuan dari proyek ini adalah untuk mengembangkan sistem yang mampu mendeteksi stomata secara otomatis pada citra daun mikroskopis menggunakan pendekatan pemrosesan citra klasik (classical computer vision), tanpa menggunakan library deep learning seperti TensorFlow, Keras, atau PyTorch.

## Deskripsi Umum

Stomata merupakan pori-pori kecil pada daun yang berperan penting dalam pertukaran gas dan pengaturan transpirasi pada tumbuhan. Deteksi otomatis stomata sangat berguna untuk mempercepat proses penelitian dalam bidang botani, fisiologi tanaman, dan studi adaptasi lingkungan. Sistem yang dibangun dalam proyek ini memanfaatkan transformasi grayscale, smoothing Gaussian, peningkatan kontras, deteksi tepi Sobel, segmentasi threshold Otsu, serta operasi morfologi dan ekstraksi fitur geometris untuk mendeteksi stomata secara akurat.

## Fitur Utama

- Deteksi objek stomata dari citra RGB mikroskopis.
- Implementasi algoritma pengolahan citra klasik tanpa pustaka deep learning.
- Visualisasi tahapan pemrosesan citra secara lengkap.
- Ekstraksi dan validasi fitur objek berdasarkan ukuran, bentuk, dan rasio.

## Metode yang Digunakan

1. Konversi citra RGB ke grayscale.
2. Peredaman noise menggunakan Gaussian smoothing (kernel 5x5, sigma 1.2).
3. Peningkatan kontras menggunakan transformasi linier.
4. Deteksi tepi menggunakan operator Sobel.
5. Segmentasi biner menggunakan metode thresholding Otsu.
6. Operasi morfologi: opening, closing, dan pengisian area objek.
7. Ekstraksi fitur objek: area, circularity, dan aspect ratio.
8. Visualisasi hasil deteksi pada citra asli.

## Cara Menjalankan (Google Colab)

1. Buka [Google Colab](https://colab.research.google.com).
2. Salin kode dari file `deteksi_stomata.py` ke dalam sel baru, atau unggah file Python tersebut.
3. Jalankan seluruh sel.
4. Sistem akan meminta pengguna untuk mengunggah citra daun mikroskopis dalam format `.jpg` atau `.png`.
5. Proses deteksi akan dilakukan dan hasil ditampilkan secara visual.


## Parameter Utama

- Ukuran kernel Gaussian: 5x5
- Nilai sigma: 1.2
- Alpha (kontras): 1.3
- Beta (kontras): 20
- Rentang area valid: 80 - 600 piksel
- Circularity valid: 0.3 - 0.9
- Aspect ratio valid: 0.4 - 2.5


## Penulis

Nama : Aurency Christabella Lolo  
NIM  : D121221074  
Mata Kuliah Visi Komputer – Semester Genap 2024/2025  

