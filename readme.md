# 📊 JSON to Excel Converter & Table Previewer

Aplikasi berbasis web yang ringan, cepat, dan aman untuk mengonversi data **JSON ke spreadsheet Excel (`.xlsx`)** dengan fitur **pratinjau tabel interaktif (*interactive preview*)** sebelum data diunduh.

Dibuat sepenuhnya di sisi peramban (*100% client-side*), sehingga data sensitif Anda tidak pernah dikirimkan ke server pihak ketiga mana pun.

---

## ✨ Fitur Utama

- **👁️ Pratinjau Tabel Interaktif:** Periksa, telaah, dan verifikasi struktur baris & kolom data terlebih dahulu sebelum mengunduhnya.
- **📥 Ekspor Instan ke Excel (`.xlsx`):** Konversi data array of objects ke format spreadsheet standar secara presisi menggunakan SheetJS.
- **🔍 Pencarian Real-Time:** Filter dan cari teks tertentu di seluruh baris tabel pratinjau secara instan.
- **🧹 JSON Auto-Formatter & Reset:** Rapikan indentasi JSON yang berantakan atau bersihkan input hanya dengan satu klik.
- **⚡ Contoh Data Siap Pakai:** Coba langsung fungsionalitas aplikasi dengan tombol *"Muat Contoh Data"*.
- **📐 Tata Letak 2 Kolom Responsif:** Sidebar input JSON di sisi kiri dan area tabel pratinjau yang luas di sisi kanan dengan *sticky header*.
- **🔒 Privasi Terjamin:** Semua proses parsing JSON dan generasi file Excel berlangsung di browser pengguna (*no backend, zero tracking*).

---

## 🚀 Demo & Cara Menjalankan

Aplikasi ini tidak memerlukan instalasi dependensi (Node.js/npm) maupun proses *build*.

### 1. Jalankan Langsung di Komputer Lokal
1. Unduh atau clone repositori ini:
   ```bash
   git clone https://github.com/username/json-to-excel-converter.git
   ```
2. Masuk ke folder proyek:
   ```bash
   cd json-to-excel-converter
   ```
3. Buka file `index.html` langsung menggunakan browser favorit Anda (Google Chrome, Firefox, Edge, Safari), atau jalankan via ekstensi *Live Server* di VS Code.

### 2. Deploy ke GitHub Pages (Gratis)
1. Push file `index.html` ke repositori GitHub Anda.
2. Buka menu **Settings** > **Pages** di repositori.
3. Pada opsi **Branch**, pilih `main` (atau `master`) dan folder `/root`, lalu klik **Save**.
4. Website Anda siap diakses secara online dalam hitungan detik!

---

## 📖 Panduan Penggunaan

1. **Tempelkan Data JSON** pada kolom teks di panel sebelah kiri.
   - Anda dapat menekan tombol **"Rapikan"** jika format JSON belum terindentasi dengan baik.
2. Klik tombol biru **"Pratinjau Tabel"** untuk menampilkan data dalam bentuk tabel interaktif di sebelah kanan.
3. Gunakan kotak **"Cari dalam tabel..."** untuk memfilter baris data jika diperlukan.
4. Jika data sudah sesuai, klik tombol hijau **"Unduh Excel (.xlsx)"** untuk menyimpan file spreadsheet ke komputer Anda.

---

## 📋 Contoh Format JSON yang Didukung

Aplikasi mendukung format array objek standar, misalnya:

```json
[
  {
    "id": "EMP-001",
    "nama": "Budi Santoso",
    "departemen": "Teknologi",
    "posisi": "Senior Engineer",
    "gaji": 15000000,
    "status": "Aktif"
  },
  {
    "id": "EMP-002",
    "nama": "Siti Rahma",
    "departemen": "Desain",
    "posisi": "UI/UX Designer",
    "gaji": 12500000,
    "status": "Aktif"
  }
]
```

> **Catatan:** Jika Anda memasukkan satu objek tunggal `{ ... }`, aplikasi akan secara otomatis membungkusnya menjadi array 1 baris agar tetap dapat ditampilkan di tabel dan diekspor ke Excel.

---

## 🛠️ Teknologi yang Digunakan

- **HTML5 & Vanilla JavaScript (ES6+)** – Logika parsing JSON, manipulasi DOM, dan filter pencarian.
- **[Tailwind CSS (CDN)](https://tailwindcss.com/)** – Penataan antarmuka modern, responsif, dan rapi.
- **[SheetJS / xlsx](https://sheetjs.com/)** – Pustaka pembuat dan pengekspor file spreadsheet Excel.

---

## 🤝 Kontribusi

Kontribusi, saran perbaikan, dan *pull request* sangat terbuka!
1. Fork repositori ini
2. Buat branch fitur baru (`git checkout -b fitur/fitur-baru`)
3. Commit perubahan Anda (`git commit -m 'Menambahkan fitur baru'`)
4. Push ke branch Anda (`git push origin fitur/fitur-baru`)
5. Buat **Pull Request**

---

## 📄 Lisensi

Didistribusikan di bawah Lisensi **MIT**. Silakan gunakan, modifikasi, dan bagikan secara bebas.