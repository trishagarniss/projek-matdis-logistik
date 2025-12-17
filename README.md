# 🚚 Optimasi Rute & Estimasi Waktu Logistik Berbasis Matdis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange)
![Status](https://img.shields.io/badge/Status-Research-green)

> **Judul:** Optimasi Rute dan Estimasi Waktu Pengiriman Logistik Menggunakan Representasi Graf Berbobot Dinamis (*Dynamic Weighted Graph*) Berbasis Logika Predikat pada Kondisi Lalu Lintas dan Cuaca.

Repository ini berisi *source code* simulasi dan dataset untuk Tugas Akhir Mata Kuliah **Matematika Diskrit**. Proyek ini bertujuan memecahkan masalah ketidakakuratan estimasi waktu pengiriman (*Last-Mile Delivery*) akibat faktor dinamis.

---

## 🧩 Konsep Sistem (Statis vs Dinamis)

Sistem ini mengubah cara pandang navigasi konvensional:
* **Statis (Biasa):** "Jarak 5 KM = 10 Menit."
* **Dinamis (Sistem Kami):** "Jarak 5 KM, tapi karena **Badai (Stormy)** dan **Macet (Jam)**, waktu tempuh menjadi **35 Menit**."

### Alur Program:
1.  **Input:** Data pesanan (Lokasi A ke B, Cuaca, Traffic).
2.  **Graf Spasial:** Menghitung jarak fisik menggunakan rumus **Haversine**.
3.  **Logika Adaptif:** Menggunakan **Logika Predikat** (Aturan *IF-THEN*) untuk memberikan penalti waktu jika kondisi lingkungan buruk.
4.  **Seleksi Kurir:** Menggunakan **Teori Himpunan** untuk memilih kurir yang paling sesuai (Irisan antara Rating & Kesiapan Kendaraan).

---

## 📚 Penerapan Materi Matematika Diskrit

| Materi | Implementasi pada Proyek |
| :--- | :--- |
| **1. Teori Graf (Utama)** | Representasi peta rute (Titik & Garis) dan perhitungan bobot jarak fisik. |
| **2. Logika Matematika** | Logika Predikat untuk konversi kondisi cuaca/macet menjadi variabel waktu. |
| **3. Teori Himpunan** | Filtering dan seleksi armada kurir (Operasi Irisan). |
| **4. Fungsi** | Pemetaan input deterministik (Jarak, Cuaca) menjadi output (Waktu). |
| **5. Tree (Pohon)** | Struktur penelusuran algoritma pencarian jalur (*Spanning Tree*). |

---

## 👥 Tim 3

* **Trisha Garnis Wahningyun** (L0224012)
* **Nadhifa Sakha Tri Yasmin** (L0224036)
* **Kayla Maharani Muzaki** (L0224050)

---

## 🚀 Cara Menjalankan

1.  **Clone Repository**
    ```bash
    git clone https://github.com/trishagarniss/projek-matdis-logistik.git
    ```
2.  **Install Library**
    ```bash
    pip install pandas numpy matplotlib folium jupyter
    ```
3.  **Jalankan Jupyter Notebook**
    Buka file `notebooks/run_simulation.ipynb`.

---

## 🔗 Referensi Utama

1.  **Shuaibu et al. (2025)** - *Last-Mile Delivery Optimization: Recent Approaches and Advances.*
2.  **Osuna-Coutiño et al. (2025)** - *Fuzzy Linear Programming Formulation for Time Prediction in Product Delivery.*
3.  **Panday & Adinda (2022)** - *Assignment Optimization of Courier Services.*
