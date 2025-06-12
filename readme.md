# 🥗 Nutrilance - Sistem Rekomendasi Diet Makanan Berbasis Website

## 📌 Deskripsi Singkat

*Nutrilance* (singkatan dari Nutrition Balance) adalah aplikasi berbasis web yang dikembangkan sebagai solusi cerdas untuk memberikan rekomendasi makanan harian yang sesuai dengan kebutuhan nutrisi pengguna. Sistem ini menggabungkan data input dari pengguna dengan model Machine Learning untuk menghasilkan saran makanan yang seimbang dan mudah diakses oleh siapa saja.

---

## 📚 Daftar Isi

- [Latar Belakang](#latar-belakang)
- [Fitur Utama](#fitur-utama)
- [Teknologi yang Digunakan](#teknologi-yang-digunakan)
- [Struktur Proyek](#struktur-proyek)
- [Instalasi dan Menjalankan](#instalasi-dan-menjalankan)
- [Contoh Penggunaan](#contoh-penggunaan)
- [Evaluasi Model](#evaluasi-model)
- [Rencana Pengembangan](#rencana-pengembangan)
- [Kontributor](#kontributor)
- [Lisensi](#lisensi)

---

## 🧠 Latar Belakang

Saat ini masih banyak masyarakat yang mengalami kesulitan dalam menentukan makanan sehat yang sesuai dengan kebutuhan nutrisinya. Tidak semua orang memiliki akses ke ahli gizi, dan kebanyakan aplikasi yang tersedia hanya fokus pada pelacakan kalori, bukan rekomendasi aktif.

Oleh karena itu, *Nutrilance* dikembangkan untuk:

- Memberikan *rekomendasi makanan berbasis data* lokal.
- Memperhitungkan input pribadi seperti berat badan, tinggi badan, aktivitas, dan tujuan diet.
- Menawarkan pengalaman yang ringan, praktis, dan informatif.

---

## 🌟 Fitur Utama

- Input data pengguna (berat, tinggi, usia, aktivitas fisik)
- Hitung kebutuhan kalori harian secara otomatis
- Rekomendasi makanan berdasarkan kebutuhan kalori & nutrisi
- Tampilan hasil dengan informasi gizi dan total kalori
- Desain web responsif dan mudah digunakan

---

## 🛠 Teknologi yang Digunakan

- *Python* - Bahasa pemrograman utama untuk model ML
- *Pandas, Scikit-learn* - Untuk analisis dan model ML (Content-Based Filtering)
- *Flask* - Backend API
- *HTML, CSS, JavaScript* - Frontend website
- *SQLite/MySQL (Opsional)* - Untuk menyimpan data pengguna (jika diperlukan)

---

## 📁 Struktur Proyek
Nutrilance/
│
├── app/ # Folder aplikasi Flask
│ ├── static/ # File CSS/JS
│ ├── templates/ # File HTML (Jinja)
│ ├── model.py # Model rekomendasi makanan
│ └── app.py # Main Flask app
│
├── data/ # Dataset makanan & nutrisi
│ └── food.csv
│
├── README.md # Dokumentasi proyek
├── requirements.txt # Library yang dibutuhkan
└── utils.py # Fungsi pendukung
---

## ⚙ Instalasi dan Menjalankan

1. *Clone repo:*
   ```bash
   git clone https://github.com/username/Nutrilance.git
   cd Nutrilance

   Buat virtual environment (opsional):

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # atau venv\Scripts\activate untuk Windows

