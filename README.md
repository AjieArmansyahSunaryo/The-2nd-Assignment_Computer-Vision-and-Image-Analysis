# CVL_Assignment02: Object Detection from Scratch

## Nama: Ajie Armansyah Sunaryo
## NIM: 24/545286/PA/23170

Repositori ini berisi implementasi algoritma deteksi objek yang dibangun dari awal (*from scratch*) tanpa menggunakan *library* *machine learning* atau *computer vision* tingkat tinggi seperti OpenCV, TensorFlow, atau PyTorch. 

Proyek ini dibuat sebagai bagian dari tugas eksplorasi algoritma Computer Vision dasar.

## Deskripsi Proyek

Tujuan utama dari proyek ini adalah untuk memahami konsep dasar bagaimana komputer mendeteksi sebuah objek dalam gambar. Metode yang digunakan adalah **Sliding Window Template Matching**. Algoritma akan memindai gambar piksel demi piksel untuk mencari area yang memiliki kemiripan tertinggi dengan *template* objek yang dicari menggunakan perhitungan *Sum of Squared Differences (SSD)*.

Untuk memastikan *notebook* dapat berjalan secara mandiri (*standalone*) dan direproduksi dengan mudah tanpa perlu mengunduh *dataset* eksternal, proyek ini menggunakan **gambar sintesis** yang di-generate langsung menggunakan NumPy.

## Fitur Utama

1. **Sliding Window Algorithm:** Implementasi pergeseran jendela secara manual pada matriks gambar.
2. **Template Matching:** Penggunaan metrik *Sum of Squared Differences (SSD)* untuk mencari kecocokan piksel.
3. **Manual Evaluation Metrics:** Implementasi perhitungan metrik evaluasi deteksi objek secara matematis dari awal:
   - *Intersection over Union (IoU)*
   - Akurasi (berdasarkan ambang batas / *threshold* IoU standar)
4. **Visualisasi Bounding Box:** Penggambaran kotak *Ground Truth* dan kotak Prediksi menggunakan Matplotlib.
