# Speech Classification with CNN

Proyek ini adalah sistem klasifikasi audio berbasis Python menggunakan PyTorch dan Librosa, yang bertujuan untuk mengenali 5 jenis suara tiruan hewan. Proyek ini terdiri dari tiga tahap utama:
1.  **Pengambilan Sampel Audio**
2.  **Pelatihan Model CNN**
3.  **Klasifikasi Suara secara Realtime**

## 📁 Struktur Folder

.

├── data/ # Menyimpan sampel audio yang direkam

├── speech_classification.ipynb # Notebook utama untuk training & klasifikasi

├── speech_cnn.pth # Model .pth yang telah dilatih

└── README.md

## 🔧 Instalasi

1.  Clone repositori ini:
    ```bash
    git clone https://github.com/DevinFaiz/speech_classification.git

    cd speech_classification
    ```

2.  Install dependencies:

    ```bash
    pip install torch numpy librosa sounddevice soundfile matplotlib scikit-learn
    ```
    (Catatan: Pastikan versi PyTorch sesuai dengan instalasi CUDA Anda jika menggunakan GPU).

## 🚀 Cara Menjalankan

Seluruh alur kerja proyek terdapat di dalam file `speech_classification.ipynb`.

### 1. Rekam Dataset Suara
* Jalankan sel-sel di notebook hingga bagian perekaman data.
* Ikuti instruksi untuk merekam 15 sampel untuk masing-masing dari 5 kelas suara: `moo`, `meow`, `woof`, `mbee`, `tweet`.
* File audio akan disimpan secara otomatis di dalam folder `data/`.

### 2. Latih Model
* Lanjutkan menjalankan sel-sel berikutnya di notebook.
* Skrip akan melakukan pre-processing, ekstraksi fitur MFCC, dan melatih model CNN.
* Model yang telah dilatih akan disimpan sebagai `speech_cnn.pth`.

### 3. Klasifikasi Suara
* Jalankan sel terakhir pada notebook.
* Sistem akan meminta Anda untuk membuat suara, kemudian akan menampilkan probabilitas untuk setiap kelas dan hasil prediksi akhirnya.

## 🧠 Teknologi yang Digunakan
* **Python**
* **PyTorch**
* **Librosa**
* **SoundDevice**
* **NumPy**
* **Scikit-learn**