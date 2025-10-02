# 🎥 Deteksi Jari & Angka

Aplikasi web untuk mendeteksi jari dan angka menggunakan kamera dengan teknologi Machine Learning berbasis Teachable Machine dari Google.

## 📋 Deskripsi

Proyek ini adalah aplikasi web yang dapat mendeteksi gerakan jari dan angka melalui kamera menggunakan model Machine Learning yang telah dilatih dengan Teachable Machine. Aplikasi memiliki fallback mode untuk menjalankan kamera tanpa deteksi ML jika model tidak tersedia.

## ✨ Fitur

- 🎯 Deteksi real-time jari dan angka
- 📱 Responsif untuk desktop dan mobile
- 🎨 UI dengan tema warna krem yang elegan
- 🔄 Mode fallback jika model ML tidak tersedia
- 📊 Progress bar untuk setiap kategori prediksi
- ⚡ Performance yang optimal dengan TensorFlow.js

## 🛠️ Teknologi yang Digunakan

- **HTML5** - Struktur aplikasi
- **CSS3** - Styling dengan tema krem yang modern
- **JavaScript (ES6+)** - Logic aplikasi
- **Bootstrap 5.3.0** - Framework CSS untuk responsivitas
- **TensorFlow.js 3.20.0** - Machine Learning di browser
- **Teachable Machine** - Platform untuk training model
- **WebRTC** - Akses kamera browser

## 🚀 Cara Menggunakan

### Prerequisites
- Browser modern yang mendukung WebRTC (Chrome, Firefox, Safari, Edge)
- Koneksi internet untuk memuat libraries dan model
- Kamera yang dapat diakses browser

### Langkah-langkah:

1. **Buka aplikasi**
   ```
   Buka file ML test .html di browser
   ```

2. **Izinkan akses kamera**
   - Klik tombol "Mulai Kamera"
   - Berikan izin akses kamera saat diminta browser

3. **Mulai deteksi**
   - Tunjukkan jari atau angka ke kamera
   - Lihat hasil prediksi di panel sebelah kanan
   - Progress bar menunjukkan tingkat keyakinan untuk setiap kategori

4. **Stop aplikasi**
   - Klik tombol "Stop Kamera" untuk menghentikan

## 📁 Struktur File

```
ML test .html          # File utama aplikasi
README.md             # Dokumentasi proyek (file ini)
```

## ⚙️ Konfigurasi

### Mengganti Model ML

Untuk menggunakan model Teachable Machine Anda sendiri:

1. Latih model di [Teachable Machine](https://teachablemachine.withgoogle.com/)
2. Export model sebagai "TensorFlow.js"
3. Ganti URL model di file [`ML test .html`](ML test .html):

```javascript
const URL = "https://teachablemachine.withgoogle.com/models/YOUR-MODEL-ID/";
```

### Customisasi Tampilan

Anda dapat mengubah tema warna dengan memodifikasi variabel CSS:

```css
/* Warna background utama */
background-color: #fdf6e3;

/* Warna teks */
color: #4e342e;

/* Warna tombol */
background-color: #6d4c41;
```

## 🎯 Mode Operasi

### 1. Mode ML (Normal)
- Memuat model dari Teachable Machine
- Melakukan prediksi real-time
- Menampilkan confidence score untuk setiap kategori

### 2. Mode Camera Only (Fallback)
- Aktif jika model tidak dapat dimuat
- Hanya menampilkan feed kamera
- Berguna untuk testing akses kamera

## 🚨 Troubleshooting

### Kamera tidak dapat diakses
- Pastikan browser mendukung WebRTC
- Berikan izin akses kamera
- Periksa apakah kamera tidak digunakan aplikasi lain

### Model tidak dapat dimuat
- Periksa koneksi internet
- Pastikan URL model valid
- Aplikasi akan otomatis fallback ke mode kamera saja

### Performance lambat
- Tutup tab browser lain
- Gunakan browser dengan hardware acceleration
- Pastikan pencahayaan cukup untuk deteksi optimal

## 📱 Kompatibilitas Browser

| Browser | Desktop | Mobile |
|---------|---------|--------|
| Chrome  | ✅      | ✅     |
| Firefox | ✅      | ✅     |
| Safari  | ✅      | ✅     |
| Edge    | ✅      | ✅     |

## 🤝 Kontribusi

Untuk berkontribusi pada proyek ini:

1. Fork repository
2. Buat branch fitur baru
3. Commit perubahan
4. Push ke branch
5. Buat Pull Request

## 📞 Support

Jika mengalami masalah atau memiliki pertanyaan:

- Periksa console browser untuk error messages
- Pastikan semua dependencies ter-load dengan benar
- Cek dokumentasi [Teachable Machine](https://teachablemachine.withgoogle.com/)

## 📄 Lisensi

Proyek ini menggunakan libraries open source:
- TensorFlow.js (Apache 2.0)
- Bootstrap (MIT)
- Teachable Machine (Apache 2.0)

---

**Dibuat dengan ❤️ untuk pembelajaran Machine Learning**