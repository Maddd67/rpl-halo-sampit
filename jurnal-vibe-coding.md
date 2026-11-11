# Jurnal Vibe Coding — Jobsheet 1
- **Nama:** [Akhmad Aulia Nuur]
- **NIM:** [24554010025]
- **Kelas:** [Rekayasa Perangkat Lunak]

| No | Tujuan | Prompt (ringkas) | Hasil AI | Keputusan | Alasan |
|---|---|---|---|---|---|
| 1 | Beranda + formulir nama | Konteks Flask "Halo Sampit", beranda dengan judul, waktu server, formulir nama, dan sapaan balik tanpa DB/JS | Menghasilkan `app.py` dan `templates/index.html` terpisah | **Terima** | Kode bersih, menggunakan Jinja2 escaping otomatis, dan sesuai spesifikasi tanpa dependensi berlebih. |
| 2 | Tambah fungsi salam sesuai waktu | Tambahkan fungsi `salam_waktu(jam)` (Pagi/Siang/Sore/Malam) dan tampilkan di beranda sebelum waktu server | Menambahkan fungsi `salam_waktu` dan memperbarui konteks render templat | **Terima** | Pengujian logis jam 3, 4, 10, 11, 14, 15, 17, 18 mengembalikan nilai salam yang tepat sesuai kriteria. |
| 3 | Tambah halaman /tentang | Tambahkan rute `/tentang` dan file `tentang.html` berisi nama, NIM, kelas, kelompok, serta navigasi balik | Menghasilkan rute rujukan baru dan berkas HTML `tentang.html` | **Terima** | Rute berfungsi dengan baik dan navigasi dua arah berjalan lancar. |
| 4 | Validasi nama di server-side | Tambahkan pembatasan panjang nama maksimal 50 karakter di sisi server (`app.py`) | Memotong string nama menggunakan *slicing* `[:50]` di fungsi `beranda()` | **Terima** | Mampu mencegah bypass `maxlength` HTML dari Inspect Element. |