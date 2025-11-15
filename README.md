# metode-manipulasi-citra-digital

Adaptive Image Enhancement menggunakan CLAHE (Contrast Limited Adaptive Histogram Equalization)
Proyek ini menerapkan metode CLAHE (Contrast Limited Adaptive Histogram Equalization) untuk meningkatkan kualitas visual citra pada domain spasial. Metode ini sering digunakan untuk memperbaiki kontras gambar tanpa merusak warna atau menambah noise berlebihan.
CLAHE merupakan pengembangan dari AHE (Adaptive Histogram Equalization) dengan penambahan batas (clip limit) agar hasil tetap natural.

**Tujuan**

Meningkatkan detail pada gambar yang memiliki pencahayaan tidak merata.

Memperbaiki kontras lokal tanpa merusak bagian terang dan gelap.

Menghasilkan tampilan citra yang lebih jelas namun tetap natural.

**Kenapa Menggunakan CLAHE?**

Dibandingkan metode lain seperti Brightness/Contrast, Gamma Correction, AHE, atau ACE:

Brightness/Contrast: hasil terlalu sederhana

Gamma Correction: hanya cocok untuk terlalu gelap/terang

AHE: meningkatkan noise secara signifikan

ACE: cenderung menghasilkan tekstur kasar pada gambar biasa

**CLAHE:**

✔ Natural
✔ Mengurangi noise
✔ Detail muncul
✔ Cocok untuk foto nyata
Itulah sebabnya CLAHE menjadi pilihan terbaik untuk enhancement citra pada project ini.

**Cara Kerja CLAHE Singkat**

Gambar diubah ke ruang warna LAB

L = Lightness (kecerahan)

A = channel hijau-merah

B = channel biru-kuning

CLAHE diterapkan hanya pada channel L
→ memperbaiki kontras tanpa merusak warna.

Gambar digabungkan kembali dan dikonversi ke RGB.

**Cara Menjalankan Program**

Pastikan Python 3 terinstall

Install library yang dibutuhkan: pip install opencv-python matplotlib numpy

Pastikan gambar (img-1.jpeg) berada di folder yang sama dengan main.py

Jalankan program: python main.py

**Output**

Program akan menampilkan dua gambar:

Original

Enhanced (CLAHE)

Hasil enhancement menunjukkan peningkatan kontras yang lebih natural tanpa penambahan noise berlebihan.

**Lisensi**

Proyek ini dibuat untuk kebutuhan pembelajaran mata kuliah Pengolahan Citra Digital.
