# GAN-Based-Coffee-Bean-Classifier
## Gambaran Umum Proyek
Proyek ini bertujuan untuk membangun sistem klasifikasi biji kopi yang akurat menggunakan Generative Adversarial Networks (GAN). Metode tradisional seringkali menghadapi keterbatasan dataset yang kecil atau tidak seimbang, yang dapat memengaruhi kinerja model. Untuk mengatasi hal ini, kami menggunakan GAN untuk menghasilkan gambar biji kopi sintetis yang realistis. Gambar-gambar hasil sintesis ini kemudian digabungkan dengan dataset asli untuk melatih model klasifikasi yang lebih tangguh dan akurat.

## Fitur Utama
- Dataset Generasi GAN: Menggunakan GAN untuk menciptakan data gambar biji kopi baru.
- Model Klasifikasi: Membandingkan performa model klasifikasi berbasis Deep Learning (ResNet, EfficientNet, MobileNet dan VGG) yang dilatih pada dataset sintetis, dataset original dan dataset gabungan.
- Performa: Dengan adanya data sintetis, kita dapat melihat pengaruh performa klasifikasi dan menetukan perlakuan terbaik untuk menghasilkan akurasi terbaik.

## Teknologi yang Digunakan
- Bahasa Pemrograman: Python
- Framework: PyTorch
- Library: NumPy, Matplotlib, scikit-learn, PIL etc.

## Struktur Repositori
```
├── data/
│   ├── original/         # Dataset biji kopi asli
│   └── synthetic/        # Dataset hasil sintesis GAN
├── Code/
│   ├── GAN_data_generation.py # Code untuk melatih GAN
│   └── Classifier_training.py # Code untuk melatih classifier
├── models/
│   ├── gan_generator.h5        # Model generator GAN yang sudah dilatih
│   └── classifier_model.h5     # Model classifier yang sudah dilatih
├── README.md               # Deskripsi repositori ini
└── requirements.txt        # Daftar library yang dibutuhkan
```

## Cara Menjalankan Proyek
1.  **Clone repositori**:
    ```bash
    git clone [https://github.com/nama-pengguna-anda/GAN-Based-Coffee-Bean-Classifier.git](https://github.com/nama-pengguna-anda/GAN-Based-Coffee-Bean-Classifier.git)
    cd GAN-Based-Coffee-Bean-Classifier
    ```
2.  **Instal dependensi**:
    ```bash
    pip install -r requirements.txt
    ```
3.  **Jalankan notebook** `GAN_data_generation.ipynb` untuk menghasilkan data sintetis.
4.  **Jalankan notebook** `Classifier_training.ipynb` untuk melatih dan menguji model klasifikasi.


