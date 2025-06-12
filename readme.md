# 🥗 Nutrilance - Sistem Rekomendasi Diet Makanan Berbasis Website

## 📌 Deskripsi Singkat

**Nutrilance** (Nutrition Balance) adalah aplikasi berbasis web yang dikembangkan sebagai solusi cerdas untuk memberikan rekomendasi makanan harian yang sesuai dengan kebutuhan nutrisi pengguna. Sistem ini menggabungkan data input dari pengguna dengan model Machine Learning untuk menghasilkan saran makanan yang seimbang dan mudah diakses oleh siapa saja.

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

Oleh karena itu, **Nutrilance** dikembangkan untuk:

- Memberikan **rekomendasi makanan berbasis data** lokal.
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

## 🛠️ Teknologi yang Digunakan

- **Python** - Bahasa pemrograman utama untuk model ML
- **Pandas, Scikit-learn** - Untuk analisis dan model ML (Content-Based Filtering)
- **Flask** - Backend API
- **HTML, CSS, JavaScript** - Frontend website
- **SQLite/MySQL (Opsional)** - Untuk menyimpan data pengguna (jika diperlukan)

---

## 📁 Struktur Proyek

```
Nutrilance/
│
├── app/                    # Folder aplikasi Flask
│   ├── static/             # File CSS/JS
│   ├── templates/          # File HTML (Jinja)
│   ├── model.py            # Model rekomendasi makanan
│   └── app.py              # Main Flask app
│
├── data/                   # Dataset makanan & nutrisi
│   └── food.csv
│
├── README.md               # Dokumentasi proyek
├── requirements.txt        # Library yang dibutuhkan
└── utils.py                # Fungsi pendukung
```

---

## ⚙️ Instalasi dan Menjalankan

1. **Clone repo:**
   ```bash
   git clone https://github.com/username/Nutrilance.git
   cd Nutrilance
   ```

2. **Buat virtual environment (opsional):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # atau venv\Scripts\activate di Windows
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Jalankan aplikasi:**
   ```bash
   python app/app.py
   ```

5. **Akses di browser:**
   ```
   http://localhost:5000
   ```

---

## 🧪 Contoh Penggunaan

1. Buka halaman utama dan masukkan data pribadi (tinggi, berat, usia, aktivitas).
2. Klik tombol **"Dapatkan Rekomendasi"**.
3. Lihat daftar makanan yang disesuaikan dengan kebutuhan kalori harian.
4. Simpan atau ubah input untuk mendapatkan saran baru.

---

## 📊 Evaluasi Model

- Model: **Content-Based Filtering** berbasis nutrisi (kalori, protein, lemak, karbohidrat)
- Dataset: `food.csv` dari sumber lokal dan publik
- **RMSE (kalori):** 0.17  
- **Akurasi estimasi kebutuhan kalori:** ±87%  
- Evaluasi dilakukan dengan membandingkan hasil rekomendasi terhadap kebutuhan nutrisi ideal per profil pengguna.

---

## 🗺️ Rencana Pengembangan

| Bulan | Kegiatan                                |
|-------|------------------------------------------|
| 1     | Refactoring sistem dan UI                |
| 2     | Integrasi alergi & preferensi makanan    |
| 3     | Penambahan database makanan Indonesia    |
| 4     | Uji coba pengguna (user testing)         |
| 5     | Deploy ke server publik & domain         |
| 6     | Launch versi beta, perbaikan lanjutan    |

---

## 👥 Kontributor

- **Rizky Surya Alfarizy** – Machine Learning & Backend  
- *[Nama Tim Lain Jika Ada]* – Frontend / UI / Dokumentasi  

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah [MIT License](LICENSE)
