# Sistem Pelacakan Alumni Otomatis Berbasis Sumber Publik

Proyek ini adalah prototipe aplikasi web untuk melakukan pelacakan rekam jejak alumni melalui sumber publik (seperti LinkedIn, Google Scholar, dll). Sistem ini mengotomatisasi pencarian, ekstraksi sinyal identitas, disambiguasi, dan penentuan status pelacakan.

## Tautan Proyek
- **Source Code (GitHub):** https://github.com/enno04/pelacakan-alumni
- **Web Publish (Live Demo):** https://enno04.github.io/pelacakan-alumni/

## Tabel Pengujian Kualitas Aplikasi
Pengujian dilakukan berdasarkan aspek kualitas perangkat lunak (Kesesuaian Fungsional, Usability, dan Performance).

| No | Aspek Kualitas | Skenario Pengujian / Test Case | Hasil yang Diharapkan | Hasil Pengujian | Status |
|---|---|---|---|---|---|
| 1 | **Functional Suitability** | Menekan tombol "Jalankan Pelacakan" | Sistem memproses simulasi pencarian sumber publik dan mengubah status alumni (Teridentifikasi / Perlu Verifikasi). | Status berhasil berubah setelah jeda waktu pemrosesan. | **PASS** |
| 2 | **Usability** | Mengakses web melalui perangkat *mobile* (smartphone) | Tabel dan tata letak *dashboard* menyesuaikan ukuran layar (*responsive*). | Komponen *card* dan tabel tidak terpotong dan nyaman dibaca di layar kecil. | **PASS** |
| 3 | **Performance Efficiency** | Memuat halaman awal *dashboard* | Halaman dimuat dalam waktu kurang dari 2 detik tanpa *render-blocking*. | Halaman langsung termuat karena menggunakan struktur DOM yang ringan dan CDN Bootstrap. | **PASS** |
| 4 | **Reliability** | Menekan tombol pelacakan berulang kali dengan cepat | Sistem menonaktifkan (*disable*) tombol saat proses pelacakan sedang berjalan untuk mencegah eksekusi ganda. | Tombol tidak bisa diklik hingga proses *timeout* pelacakan selesai. | **PASS** |
