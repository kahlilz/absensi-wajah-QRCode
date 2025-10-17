# 🧠 Sistem Absensi QR Code

Sistem absensi sederhana berbasis **QR Code** yang dapat dijalankan di Windows maupun Linux (termasuk TV Box).  
Proyek ini dibuat sebagai bagian dari pengembangan sistem absensi ringan tanpa memerlukan deteksi wajah.

---

## 🚀 Fitur Utama
- Membuat QR Code unik untuk setiap pengguna.  
- Melakukan absensi dengan memindai QR Code melalui webcam.  
- Menyimpan data absensi ke dalam file `.csv`.  
- Ringan dan dapat dijalankan pada perangkat dengan spesifikasi rendah.

---

## 📂 Struktur Folder
absensi-wajah-QRCode/
│
├── main.py # Program utama untuk absensi
├── qr_generator.py # Membuat QR Code pengguna
├── requirements.txt # Library yang dibutuhkan
├── data/
│ ├── users.csv # Daftar pengguna
│ └── absensi.csv # Riwayat absensi
└── utils/
└── camera_utils.py # Fungsi pembacaan kamera dan deteksi QR

## ⚙️ Instalasi

1. **Clone repository ini**
   ```bash
   git clone https://github.com/kahlilz/absensi-wajah-QRCode.git
   cd absensi-wajah-QRCode
   Instal dependensi

pip install -r requirements.txt


(Opsional) Jika pyzbar error di Linux, jalankan:

sudo apt install libzbar0

🎯 Cara Penggunaan
🧍 Tambah Pengguna Baru

Jalankan:

python qr_generator.py


Masukkan nama pengguna → sistem otomatis membuat QR Code dan menyimpannya di folder data/.

📸 Absensi Menggunakan Kamera

Jalankan:

python main.py


Arahkan kamera ke QR Code yang telah dibuat.
Sistem akan menampilkan nama dan mencatat waktu absensi ke data/absensi.csv.

💡 Catatan

Proyek ini dapat dijalankan di Windows, Linux, maupun TV Box (dengan OS Linux).

Tidak memerlukan GPU.

Cocok digunakan untuk eksperimen awal sistem absensi ringan.

👨‍💻 Pengembang

Kahlil Gibran Saputra
Proyek skripsi Universitas Mulawarman — Sistem Absensi QR Code

### ✅ **Langkah Selanjutnya**
1. Simpan isi di atas ke file bernama `README.md` di folder utama project kamu.  
2. Lalu jalankan perintah berikut di terminal:
   ```bash
   git add README.md
   git commit -m "Menambahkan README.md"
   git push