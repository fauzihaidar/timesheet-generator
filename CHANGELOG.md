# Generator Timesheet Gajian: riwayat versi dan cara rollback

Setiap file `timesheet-generator_vNN.html` adalah snapshot lengkap aplikasi (satu file, berdiri sendiri).
Nomor versi juga tertulis di bagian bawah halaman aplikasi ("Versi NN").

| Versi | Perubahan utama |
|---|---|
| v09 | Template bawaan terpasang otomatis, PDF mengikuti template, remarks kegiatan kustom, unduhan browser |
| v10 | Tanggal cuti dan remarks dibatasi di dalam periode |
| v12 | Identitas (Name Of Project, Location, Nama) dan tanda tangan opsional, kotak tanda tangan diperlebar |
| v13 | Remarks "Testing Backlog" tanpa bold, jumlah baris mengikuti panjang periode |
| v14 | Remarks panjang di-wrap, tinggi baris menyesuaikan |
| v15 | Tombol Download template disembunyikan |
| v16 | Kalender lebih andal, tanda tangan default kosong |
| v17 | Validasi "template harus punya baris merah dan hitam" dihapus |
| v18 | Mendukung template Bayu (baris tanggal mulai di baris 11, tinggi baris berbeda) |
| v21 | Notifikasi unduhan di HP, remarks Weekend berupa teks (tanpa rumus Excel) |
| v22 | Upload template/tanda tangan lebih andal di HP, pesan error jelas |
| v23 | Pilihan template bawaan (Standar / Bayu) tanpa upload, gambar tanda tangan langsung dengan jari/mouse |
| v24 | Template yang DIUPLOAD mempertahankan tanda tangannya di Excel dan PDF (template bawaan tetap tanpa tanda tangan) |
| v25 | Pilihan template bawaan disembunyikan; template default = Bayu dengan nama "Timesheet Bulanan" (template Standar masih ada di kode, tersembunyi) |
| v26 | Teks petunjuk (placeholder) di kolom Name Of Project, Location, dan Nama disembunyikan (kolom kosong tetap memakai isi template) |

Catatan: v11, v19, dan v20 adalah versi perantara yang tidak disimpan sebagai file terpisah; isinya sudah tercakup di v12 dan v21.

## Cara rollback
1. Artifact (link claude.ai): minta "rollback ke vNN"; file di folder ini dipublish ulang ke link yang sama.
2. GitHub: ganti isi `index.html` dan `timesheet-generator.html` di repository `fauzihaidar/timesheet-generator` dengan file versi yang diinginkan (atau minta "gas push github" setelah rollback).

## Folder templates
Salinan template Excel yang dipakai selama pengembangan (standar, Bayu, dan standar dengan tanda tangan).
